# Ethereum-Private-Network-On-Docker
One-click deployment of an Ethereum "Proof of Authority" blockchain on docker.

Currently, the script deploys a five-node "Proof of Authority" network with two RPC endpoints and two pre-funded accounts.

# Notes
1. Only tested on an Ubuntu 22.04 LTS.
2. If you are running on a different Linux distro, you might need to install dependencies manually.
3. If you are on Windows, you must manually install dependencies, initialize the nodes, and edit the "docker-compose.yml" accordingly. (Which means THIS IS NOT FOR WINDOWS).

# Deployment
1. Execute the "installDeps.sh" with root privileges to ensure all the dependencies are installed.
2. Edit the "CHAINID" value as desired (111222333 by default).
3. Execute the "initialize.sh" to create nodes and accounts and it will initialize nodes with a generated "genesis.json" file (Edit "genesis.json" after initialization will not do any changes).
4. Edit the "docker-compose.yml" file to match your requirements (OPTIONAL, and if doing so, KNOW WHAT YOU DOING!).
5. Execute "docker-compose-up" to start the network.
6. All required information will be stored in the "chainInfo" file.
