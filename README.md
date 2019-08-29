# Yeahreum Daemon Linux Command

How do I setup a Yeahreum Daemon Linux Command (YDLC) on Ubuntu Server 18.04


# Update your Ubuntu machine.

```
sudo apt-get update
```
```
sudo apt-get upgrade
```

# Install the required dependencies.

```
 sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils python3 
```

```
 libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev libboost-all-dev 
```
```
 libboost-program-options-dev
 ```
 ```
 sudo apt-get install libminiupnpc-dev libzmq3-dev libprotobuf-dev protobuf-compiler unzip software-properties-common
```
# Install Berkeley DB.

```
 sudo add-apt-repository ppa:bitcoin/bitcoin
```

```
 sudo apt-get update
```

```
 sudo apt-get install libdb4.8-dev libdb4.8++-dev
```


# Download the YDLC and tools from Yeahreum.


```
wget "api.server.yeahreum.net/daemon/yeahreum-daemon-linux.tar.gz" -O yeahreum-daemon-linux.tar.gz
```
Manually Install
[Download daemon](https://api.server.yeahreum.net/daemon/yeahreum-daemon-linux.tar.gz)

```
wget "api.server.yeahreum.net/daemon/yeahreum-qt-linux.tar.gz" -O yeahreum-qt-linux.tar.gz
```

Manually Install
[Download GT YDLC](https://api.server.yeahreum.net/daemon/yeahreum-qt-linux.tar.gz)

# Extract the tar files.

```
tar -xzvf yeahreum-daemon-linux.tar.gz
```

```
tar -xzvf yeahreum-qt-linux.tar.gz
```

# Install the daemon and tools.
```
 sudo mv yeahreum yeahreum-cli yeahreum-tx /usr/bin/
```
# Create the config file.
```
 mkdir $HOME/.yeahreum
 ```
 ```
 nano $HOME/.yeahreum/yeahreum.conf
```

# Paste the following lines in yeahreum.conf.


 rpcuser=rpc_yeahreum
 rpcpassword=7c6ca5196c481b88011a6bcea
 rpcallowip=127.0.0.1
 rpcport=10037
 listen=1
 server=1
 addnode=yahrm.net


# Start your YDLC with the following command.

```
# yeahreum
```



