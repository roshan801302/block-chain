### Basics commands to install Golang and Fabric

```
sudo apt update
```
to update the system

```
sudo apt install golang-go
```
to install golang-go

```
sudo snap install docker
```
to install docker

```
sudo apt install git
```
to install git

```
git clone -b main https://github.com/hyperledger/fabric-samples.git
```
to install fabric-samples

```
sudo apt install curl
```
to install curl


```
cd fabric-samples
```
to get in fabric-samples

```
sudo bash
```


```
curl -sSL https://bit.ly/2ysbOFE | bash -s
```
to pull hyperledger docker images


```
cd test-network
```
to get into test-network

```
./network.sh
```
```
./network.sh up
```
to up the network

```
./network.sh createChannel
```
to create channel

```
./network.sh down
```
to down the network

```
wget https://dist.ipfs.tech/kubo/v0.32.1/kubo_v0.32.1_linux-amd64.tar.gz
```
![image](https://github.com/user-attachments/assets/7d967d7e-f1b1-4713-b7c1-78a11124082a)


### Install IPFS

```
tar -xvzf kubo_v0.32.1_linux-amd64.tar.gz
```
to use kubo

```
cd kubo
```
to get into kubo directory

```
sudo bash install.sh
```
to move to local bin

```
ipfs init
```
to initialise ipfs

```
ipfs daemon
```
to use daemon
![image](https://github.com/user-attachments/assets/463aab2e-d535-4010-bb9a-4490111dd57b)


```
ipfs.log 2>&1 &
```
To run ipfs daemon in background

```
echo "Hello, IPFS!" > hello.txt
ipfs add hello.txt
ipfs cat <CID>
```
to add file
```
mkdir myfolder
echo "File 1 content" > myfolder/file1.txt
echo "File 2 content" > myfolder/file2.txt
ipfs add -r myfolder
```
to add a directory

```
ps aux | grep ipfs
```
lists running processes

```
kill <PID>
```
to kill the process
## encrypting and decrypting
```
echo "Hello, bruh" > myfile.txt
ipfs add myfile.txt
openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -salt -in myfile.txt -out myfile_encrypted.txt -pass pass:yourpassword
ipfs add myfile_encrypted.txt
cat myfile_encrypted.txt
openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -in myfile_encrypted.txt -out decrypted_file.txt -pass pass:yourpassword
cat decrypted_file.txt
ipfs add decrypted_file.txt
```

![image](https://github.com/user-attachments/assets/0a02b966-3f8a-4898-a421-1cf1851f4246)



## to push video and audio

```
ipfs add <audio-path>
```
to add audio



```
ipfs add <video-path>
```
to add video


## Metamask
![WhatsApp Image 2025-04-10 at 08 03 23_0c56db52](https://github.com/user-attachments/assets/36596342-719a-4de4-8db5-8787e3d783a5)

## Free Sepolia Faucet 0.05 with GCP-
![image](https://github.com/user-attachments/assets/61456c5f-9bdb-4ba0-ac39-320300a371a2)
