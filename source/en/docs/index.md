title: Asch Node Installation Guide
---

# 1. Sytem requirement
- Linux system required
- Public IP address required
- Ubuntu 14.04 64bit OS recommended
- Above dual-core CPU recommended
- Above 2 GB RAM recommended
- Above 2MB broadwidth recommended

# 2. Installation
There are two seperated systems: test version (testnet) and main official version (mainnet). Both of them are co-existed but unable to communicate with each other.

The installation procedures of these two systems are the same except the installation package and configuration file (including default port setting).

As long as there is no conflict of ports, you can install the test version and official version  on the same compouter, but please note, the power of the  computer is highly required, such as dual-core CPU, 2GB RAM above or at least 4MB brandwidth…

## 2.1 Download and unpack

For test version (testnet)

wget https://www.asch.so/downloads/asch-linux-latest-testnet.tar.gz
tar zxvf asch-linux-latest-testnet.tar.gz
For official version (mainnet)

wget https://www.asch.so/downloads/asch-linux-latest-mainnet.tar.gz
tar zxvf asch-linux-latest-mainnet.tar.gz

Usually, the version number of testnet will larger than that of mainnet.

## 2.2 Initialize
In this step,  two steps will be done automatically, as follows:
- Install some dependency modules like nodejs and sqlite3
- Install and configure the ntp service by which to synchronize your system time can be synchronized with that of other nodes.

This step only need be executed once, but it is OK to be done for several times.

Go to your installation folder
/aschd configure


# 3. Run

Go to the installation folder
To start the service
./aschd start

To stop the service
./aschd stop

To check the running status
./aschd status

To restart the service
./aschd restart

To upgrade the system
./aschd upgrade

To re-synchronize the blockchain
./aschd rebuild

To check the system version
./aschd version

To start producing block
./aschd enable "your sercret"

To check the log
tail -f logs/debug.log

# 4. Delegate configuration
## 4.1 Delegate's password

Use your favorite editor to open config.json and locate find the [secret] field. Fill this field with your delegate’s password. This field is an array of JSON format strings, which means you can set several passwords in one particular computer, but be careful not to duplicate them.

![forging secret](./assets/forging-secret.png)

NOTICE: DO NOT configure the same password, no matter in a single machine computer or in multiple machinescomputers.

## 4.2 Public IP
By default, the system will automatically detect the public IP you assigned automatically. But in some Cloud hostshost built on cloud, the public IP may not be able to identifiedidentify. Under such circumstanceIn this situation, the following field needs to be appended in config.json:

"publicIp": "Here is your public IP",

And don’t forget to restarting your system after configuration by:

./aschd restart


# 5. Upgrade the system

./aschd upgrade
./aschd start

# 6. Troubleshooting
## 6.1  I cannot access my online wallet
###  Solution 1
Check the [port] field in config.json, the default port numbers of testnet and mainnet are 4096 and 8192, respectively.

###  Solution 2
Check whether the service server is runningstarted by typing commands as follows:
```
./aschd status

if  server is not startedrunning, then following message will be shown
Asch server is not running

then restart the server
./aschd restart


## 6.2 Unable to generate the block
### Solution 1
Make sure the rank of delegate is in top 101

### Solution 2
Check the error log with following commands:

grep Failed logs/debug.log

If there is an error message like this:

Failed to get public ip, block forging MAY not work!

It means the system cannot get the public IP, and you need you to configure it manually, see [4.2 Public IP]

### Solution 3
Check the error log with following commands:

grep error logs/debug.log

If there is an error message like this:
```
Failed to load delegates: Account xxxxxxxxx not found

It means that the passphrase of your account has not been registered as a delegate yet, or you started the service before it registered as a delegate. Simply restarting the service will solve the problem.

NOTICE: If your node is synchronizing the blocks, restart the system after the synchronization is finished.

./aschd restart

If the system has been restarted successfully, the following log will be found:

grep Forging logs/debug.log

Forging enabled on account: xxxxxxxxxxxxxx
```
## 6.3 Unable to synchronize the block  (blockchain growth suspend)
This issue can be confirmed by comparing the block height of your wallet and official node

First, try to restart the system:

./aschd restart

If problem is still unsolved, try to rebuild`

./aschd rebuild
