<h1 align="center"> Zeeka Network | The Chaos Testnet 1 </h1>

![image](https://user-images.githubusercontent.com/101149671/196880084-be318e37-979b-4c9e-bb14-5765ddcfc901.png)

## System Requirements:

```
 2 CPU
 4 RAM
 50 GB SSD
 Ubuntu 20.04
```

## Setup
```
sudo apt-get update && sudo apt-get upgrade
```
```
sudo apt install -y build-essential libssl-dev cmake
```
```
apt install screen
```
## Rust tool setup:

 * During installation, options 1 - 2 and 3 will appear, we choose 1.

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
![image](https://user-images.githubusercontent.com/101149671/196891892-ef3bb9b4-12f8-44fc-a062-7e008fa6c77a.png)

## İnstall Bazuka:
```
apt install git
git clone https://github.com/zeeka-network/bazuka
```
```
source "$HOME/.cargo/env"
```
## path setup:
```
cd bazuka
cargo install --path .
```
## Let's read this carefully:

 * In this command just change where I said 'KSQHKFRTseed' and save it, it's your seed
 * If you want to move the node one day, you will establish the node with this 'SEED'.

```
bazuka init --seed KSQHKFRTseed --network chaos --node 127.0.0.1:8765
```
## Now let's run our node on a different screen:

```
screen -S bazuka
```

* Here, 2 parts will be changed and the newly opened window will be entered.
 * Enter your IP number in the part I gave as `111.111.111` outside the first section, it will not change as it is the port number '8765' at the end.
 * Second part `--discord-handle "deemirfirat#2336"` enter your discord, make sure you are on zeeka's discord.
 

```
bazuka node --listen 0.0.0.0:8765 --external 111.111.111:8765 \
  --network chaos --db ~/.bazuka-chaos --bootstrap 152.228.155.120:8765 \
  --discord-handle "deemirfirat#2336"
```
## Then you will get the output as in the picture:

 * The number of active nodes will appear as 1-2-10-30-100
 * If the number of active nodes is zero, enter the zeeka discord channel and replace any thread shared in the ip channel with the bootstrap part and try again (--bootstrap `152.228.155.120`:8765)
 
 ![image](https://user-images.githubusercontent.com/101149671/196894807-5a3b4890-b45c-46eb-9f5b-9c75be02c278.png)
 
 * 0 viewing examples:

![image](https://user-images.githubusercontent.com/101149671/196895349-4abe0823-8449-41a1-bd9f-147e90c7fa2f.png)
 
 
 ## About Zeeka:

  * [Explorer link](http://152.228.155.120:8000/)
  * [Website](https://zeeka.network/)
  * [Twitter](https://twitter.com/ZeekaNetwork)
  * [Telegram](https://t.me/ZeekaNetworkTurkish)



