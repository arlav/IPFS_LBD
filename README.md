# IPFS_LBD
This is a simple repository to showcase IPFS for Linked Building Data with Topologic.
We work with Topologic as our main platform to read and write Linked Building Data. this is a very early stage prototype and it is still under heavy development, so expect things to break.


## Prerequisites
To set up you need at least two computers running IPFS, with the IPFS tookit installed.
there is no difference whether you run IPFS cmd-line or desktop, as the desktop version is just a visual wrapper around the IPFS kubo cmd-line, so all instructions apply for both. 

* Python Installation
    - python 3.12 
    - to install multiple version of python, use either anaconda or pyenv to handle the environments.
    - [Anaconda](https://anaconda.com/)
    - [PyEnv](https://github.com/pyenv/pyenv)


* Topologic 
   - [Topologic Core](https://github.com/wassimj/Topologic)
    - to install it issue "pip install topologic_core" in the shell.
   - [Topologic Py:the Python bindings for Topologic](https://github.com/wassimj/topologicpy)
    - to install it issue "pip install topologicpy" in the shell. Topologic Core is a dependency of topologic python bindings, so it will install automatically in you install Topologic Core.


* IPFS toolkit
    [IPFS toolkit source](https://github.com/emendir/IPFS-Toolkit-Python)
    [IPFS toolkit](https://pypi.org/project/IPFS-Toolkit/)

* IPFS setup
    - Install IPFS on both computers
    - Enable "Libp2pStreamMounting" in IPFS (in settings .json) by flipping "false" to "true"
    - add each peer to the other peer using ip4 addresses

    - note the Peer IDs for use in Python scripts, for example: 
    12D3KooWMu72wB1pKA1hN3yStSdT5QBZvEKAJcFSbVjPTmZ2vyks
    - run the demo-file-receiver on the receiver IPFS node: https://github.com/emendir/IPFS-Toolkit-Python/blob/master/Examples/Demo-File-Receiver.py
    - use a modified version of the demo-file-sender.py to send the files from one ipfs node ot the other.


## Contract deployment
    - Install metamask
    - acquire test eth for Sepolia
    - grab the contract from this repository
    - use remix.ethereum.org on the Sepolia network to deploy
    - test timetrace contract deployed here: https://sepolia.etherscan.io/tx/0x34b271a9c47dba9d8c7535e5bb3e4107b549dd9111c23237a3ba2373119493b1
    - 