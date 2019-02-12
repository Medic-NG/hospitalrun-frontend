### Installation ###
1. Ensure you are acting as the sudo user. If not, use: `sudo su`
1. Ensure running Linux kernel >= 3.10 `uname -msr`
1. Update system packages: `apt-get update && apt-get upgrade -y`
1. Install Docker: 
```
curl -fsSL https://get.docker.com -o get-docker.sh 
sh get-docker.sh
```
5. Install Docker Compose: <br>
```
sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```
1. Ensure Docker Compose installed properly: `which docker-compose` should return a path to the executable.
1. Make sure git is installed; usually already installed in most DO droplets: `apt-get install git -y`
1. Change directory: `cd /srv`
1. Clone the HospitalRun fork repository: `git clone https://github.com/Medic-NG/hospitalrun-frontend.git`
1. Change directory to repository folder `cd /srv/hospitalrun-frontend`
1. Bring up the containers: `docker-compose up -d`
1. Wait for the containers to pull and go online. This could take several minutes. You will know it's done once you are back in the command prompt.

### Configuration ###
1. Create a bash script to automate git pulls: `nano /root/git-pull.sh` and insert the following code into the nano editor: `
