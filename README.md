#how works one Validator and Sentry Node for Cosmos:


#I have one Sentry-Validator-Node, and two Full-nodes-NO-Validator

#For my setup i used 4 Addresses for Full-nodes-NO-Validator i trust. two mines, two for other validator fiend.

#Beware that 

#Validator Node only connect to others No-validator nodes of your choice. Trust Full nodes (NO-Validator)
#Full-Nodes-NO-Validator need to have open port in FW 46656 , 46657 for all ip, for can work in the blockchain.




#for build your sentry validator node


#open config.toml in validator node and write te ID + IP +PORT for your No-validator nodes.

#edit:

persistent_peers = "ID@IP:PORT,ID@IP2:PORT,ID@IP3:PORT,ID@IP4:PORT" 


#example 

persistent_peers = "fsdgsdhthfdgysfgtykryjkyteje@111.111.11.1:46656,saegargrtygdfdgsdtdfjydj@112.112.2.2:46656" 

#edit too

# Set true to enable the peer-exchange reactor
pex = false




#safe and open your  Firewall software from your server in Validator Node.

open TCP 46656 for 111.111.11.1 and for 112.112.2.2

#safe and restart your FW.
 #when your FW is active for sure. 

#stop and start your validator node.

#now your validator es sentry. with the amount of trusted No-Validator-Nodes that you have written in persistent_peers.

#works
