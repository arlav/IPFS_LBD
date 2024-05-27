# IPFS_LBD
This is a simple repository to showcase IPFS for Linked Building Data with Topologic.
We work with Topologic as our main platform to read and write Linked Building Data. this is a very early stage prototype and it is still under heavy development, so expect things to break.


## Prerequisites
To set up you need at least two computers running IPFS, with the IPFS tookit installed.
there is no difference whether you run IPFS cmd-line or desktop, as the desktop version is just a visual wrapper around the IPFS kubo cmd-line, so all instructions apply for both. 



    *Topologic 
    [Topologic Core](https://github.com/wassimj/Topologic)
    [Topologic Py:the Python bindings for Topologic](https://github.com/wassimj/topologicpy)


    *IPFS toolkit
    [IPFS toolkit source](https://github.com/emendir/IPFS-Toolkit-Python)
    [IPFS toolkit](https://pypi.org/project/IPFS-Toolkit/)

    *IPFS setup
    - Install IPFS on both computers
    - Enable "Libp2pStreamMounting" in IPFS (in settings .json)
    - add each peer to the other peer using ip4 addresses: It should look like this: 
/ip4/192.168.129.12/tcp/4001/p2p/12D3KooWMu72wB1pKA1hN3yStSdT5QBZvEKAJcFSbVjPTmZ2vyks
    - note the Peer IDs for use in Python scripts, for example: 
    12D3KooWMu72wB1pKA1hN3yStSdT5QBZvEKAJcFSbVjPTmZ2vyks