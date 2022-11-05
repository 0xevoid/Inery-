
<p style="font-size:14px" align="right">
<a href="https://t.me/AHNesiaNews="_blank">Join our telegram <img src="https://user-images.githubusercontent.com/50621007/183283867-56b4d69f-bc6e-4939-b00a-72aa019d1aea.png" width="30"/></a>
<a href="https://m.do.co/c/2cea00d4f9bble" target="_blank">Deploy your VPS using our referral link to get 100$ free bonus for 60 days <img src="https://user-images.githubusercontent.com/50621007/183284313-adf81164-6db4-4284-9ea0-bcb841936350.png" width="30"/></a>/
</p>

<p align="center">
  <img height="50" height="auto" src="https://user-images.githubusercontent.com/38981255/184088981-3f7376ae-7039-4915-98f5-16c3637ccea3.PNG">
</p>

# Tutorial Become a Master Node Inery Blockchain

Dokumen Innery Official :
> [Node Lite & Master](https://docs.inery.io/docs/category/lite--master-nodes)

Explorer Inery BlockChain :
> [Explorer Inery BlockChain](https://explorer.inery.io/ "Explorer Inary")
## HARDWARE 

| Component | Minimum Requirements  |
| ------------ | ------------ |
| CPU  | Intel Core i7-8700 Hexa-Core  |
| RAM | DDR4 64 GB  |
| Storage  | 2x1 TB NVMe SSD |

## SOFTWARE 

| Component | Minimum Requirements |
| ------------ | ------------ |
| OS |  Ubuntu 18.04 | 

# 1. Before Running the Testnet Account Register Node First!
[Register Account](https://testnet.inery.io/ "https://testnet.inery.io/")

 # A. How to Register an Inery Testnet Account

- Go To Link Register: [Here](https://testnet.inery.io/ "https://testnet.inery.io/")
- Fill in your data as below.!

<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200082915-562b3f51-7354-4261-b963-6cef17037acc.png">
</p>

## B. How to Get Server Name (For Contabo VPS Users)

<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200084171-c8dc1d91-1ab3-416b-ba7b-824d3fa72b56.jpg">
</p>

- Open your Contabo Account
 - Select Managamenet Reverse DNS
 - Find your IP address and copy the link that is our name server
 - IP Address: Fill with your VPS IP Address
 - Account Name: Free Username Fill
 - Enter Your Password
 - Submit Registration
 - Save your Pharse properly and correctly
 - Don't forget To Claim Faucet Select 50k INR
 - Claim
 ✅ Done

# 2. Preparation Task 1
- Install & Update Tools We Need First

```
sudo apt-get update && sudo apt install git && sudo apt install screen
```

```
sudo apt-get install -y make bzip2 automake libbz2-dev libssl-dev doxygen graphviz libgmp3-dev \
autotools-dev libicu-dev python2.7 python2.7-dev python3 python3-dev \
autoconf libtool curl zlib1g-dev sudo ruby libusb-1.0-0-dev \
libcurl4-gnutls-dev pkg-config patch llvm-7-dev clang-7 vim-common jq libncurses5
```

- On Port (Optional or Skip this)
```
ufw allow 22 && ufw allow 8888 && ufw allow 9010 && ufw enable -y
```

- Start Node
```
git clone https://github.com/inery-blockchain/inery-node
```

- Explorer BIN
```
cd inery-node
```

- Give File Permission
```
cd inery.setup
```
```
chmod +x ine.py
```
```
./ine.py --export
```
```
cd; source .bashrc; cd -
```

- Open Your Config Then Edit, Command


**NOTE:** To configure the node with your Account information, Please Look Carefully

<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200089147-5d9be881-b61f-4f75-b1c9-fd7b178d1eb7.jpg">
</p>

Make sure the data is the same as the testnet account on the account dashboard that you created earlier..!

```
cd
cd inery-node/inery.setup
```
```
cd tools
```
```
nano config.json
```
Save (ctrl+x), Type "Y" and exit (Enter)

- Start Your Blockchain Protocol

```
cd
cd inery-node/inery.setup
```
```
screen -R master
```
```
./ine.py --master
```
**Type CTRL + A + D** To walk in the background and to return to the screen, use the command `screen -Rd master` 👇
<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200090439-216640f5-2bfa-4f8f-8757-b10b7bcc4170.jpg">
</p>

- Add Peer Open on New Tab (Optional)
```
cd
cd inery-node/inery.setup/master.node/
nano genesis_start.sh
```
<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200091055-3f171059-6bf1-4ab1-bec0-e3ff4598c137.jpg">
</p>

```
--p2p-peer-address 167.235.3.147:9010 \
--p2p-peer-address 135.181.133.169:9010 \
--p2p-peer-address bis.blockchain-servers.world \
--p2p-peer-address 62.210.245.223:9010 \
--p2p-peer-address 185.144.99.30:9010 \
--p2p-peer-address 38.242.153.15:9010 \
--p2p-peer-address 75.119.150.78:9010 \
--p2p-peer-address 192.46.226.189:9010 \
--p2p-peer-address 95.217.134.209:9010 \
--p2p-peer-address 78.46.123.82:9010 \
--p2p-peer-address 161.97.153.16:9010 \
--p2p-peer-address 38.242.154.67:9010 \
--p2p-peer-address 45.10.154.235:9010 \
--p2p-peer-address 45.84.138.8:9010 \
--p2p-peer-address 45.84.138.118:9010 \
--p2p-peer-address 38.242.248.157:9010 \
--p2p-peer-address 45.84.138.209:9010 \
--p2p-peer-address 95.217.236.223:9010 \
--p2p-peer-address 86.48.2.195:9010 \
--p2p-peer-address 135.181.254.255:9010 \
--p2p-peer-address 5.161.118.114:9010 \
--p2p-peer-address 78.47.159.172:9010 \
--p2p-peer-address 45.10.154.239:9010 \
--p2p-peer-address 45.84.138.9:9010 \
--p2p-peer-address 194.163.172.119:9010 \
--p2p-peer-address 45.84.138.119:9010 \
--p2p-peer-address 45.84.138.153:9010 \
--p2p-peer-address 130.185.118.73:9010 \
--p2p-peer-address 45.84.138.247:9010 \
--p2p-peer-address 185.202.238.240:9010 \
--p2p-peer-address 194.163.161.151:9010 \
--p2p-peer-address 65.109.15.147:9010 \
--p2p-peer-address 80.65.211.208:9010 \
--p2p-peer-address 149.102.140.38:9010 \
--p2p-peer-address 38.242.149.97:9010 \
--p2p-peer-address 38.242.156.49:9010 \
--p2p-peer-address 78.187.25.69:9010 \
--p2p-peer-address 212.68.44.36:9010 \
--p2p-peer-address 38.242.159.125:9010 \
--p2p-peer-address 77.92.132.67:9010 \
--p2p-peer-address 20.213.8.11:9010 \
--p2p-peer-address 74.208.142.87:9010 \
--p2p-peer-address 38.242.235.150:9010 \
--p2p-peer-address 65.108.82.31:9010 \
--p2p-peer-address 10.182.0.15:9010 \
--p2p-peer-address 185.249.225.183:9010 \
--p2p-peer-address 167.235.141.121:9010 \
--p2p-peer-address 194.163.162.47:9010 \
--p2p-peer-address 88.198.164.163:9010 \
--p2p-peer-address 193.46.243.16:9010 \
--p2p-peer-address 38.242.159.140:9010 \
--p2p-peer-address 149.102.143.144:9010 \
--p2p-peer-address 161.97.169.27:9010 \
--p2p-peer-address 38.242.219.100:9010 \
--p2p-peer-address 45.94.209.59:9010 \
--p2p-peer-address 167.235.3.147:9010 \
--p2p-peer-address 138.68.128.123:9010 \
--p2p-peer-address 65.108.255.170:9010 \
--p2p-peer-address 38.242.156.82:9010 \
--p2p-peer-address 5.161.55.130:9010 \
--p2p-peer-address 194.163.162.155:9010 \
--p2p-peer-address 75.119.151.217:9010 \
--p2p-peer-address 168.119.100.166:9010 \
--p2p-peer-address 209.145.56.41:9010 \
--p2p-peer-address 38.242.211.194:9010 \
--p2p-peer-address 173.212.237.51:9010 \
--p2p-peer-address 161.97.169.22:9010 \
--p2p-peer-address 194.5.152.187:9010 \
--p2p-peer-address 45.141.122.178:9010 \
--p2p-peer-address 173.249.33.164:9010 \
--p2p-peer-address 128.199.164.137:9010 \
```
Save (ctrl+x), Type "Y" and exit (Enter)

**NOTE** If you have waited for block synchronization, approximately up to 1-2 days to synchronize _Patience_
<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200091830-937cc00f-d4f6-4d97-85ca-2e16c375b837.jpg">
</p>

<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200091833-1a2de92e-cbe3-41f3-9711-b2e025553bfb.jpg">
</p>

<a href="https://explorer.inery.io/" target="_blank">Inery Explorer

- Start Node
Do This Still in New TAB

```
cd ~/inery-node/inery.setup/master.node/
./start.sh
```

- Connect Wallet
Do This Still in New TAB

```
cline wallet create -n <your_name_wallet> -f file.txt
```

👇👇👇👇👇👇
<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200092832-611f074b-fb40-4d15-8530-d376dd71f6f4.jpg">
</p>

- Check Password And Save Password 
```
cd
cd inery-node/inery.setup/master.node
nano file.txt
```

**Save Your Password**

- Unlock Your Wallet

```
cline wallet unlock -n <your_name_wallet>
```
 Submit Your Password from file.txt 

👇👇👇👇👇👇
<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200094081-1f9b1c0b-fc93-435d-8714-f06aaeb10e90.jpg">
</p>

- Import Privatekey From Inery Account

```
cline wallet import --private-key <your_private_key> -n <your_name_wallet>
```
👇👇👇👇👇👇
<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200094438-f96c548f-b638-4bd3-a580-b8cae046e013.jpg">
</p>

- Register as a producer by running the command

```
cline system regproducer <your_account> <your_public_key> 0.0.0.0:9010
```
```
cline system makeprod approve <your_account> <your_account>
```
- Finished Step

<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200096170-09490909-c6a5-401c-ba2f-6e39c121d996.jpg">
</p>

Please Check In Inery Explorer, Master Node Completed!!!

### Go to Inery Account 
<p align="center">
  <img height="auto" height="auto" src="https://user-images.githubusercontent.com/112532410/200096830-edf3c979-e099-4239-a625-67836000f27b.jpg">
</p>
 - Click Task 1
 - Click Finish Task
 - Waiting approved 
 ✅ Done


## Another Commands

- Useful Commands
Check Wallet Balance
```
cline get currency balance inery.token account_name
```


- Delete Wallet at Node


***Note:*** Do not use if you are still in use ..!!

```
cline wallet stop
```
```
rm -rf inery-wallet
rm -rf file.txt
rm -rf defaultWallet.txt
```

