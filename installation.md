### Installation ###
1. Ensure you are acting as the sudo user. If not, use: `sudo su`
1. Ensure running Linux kernel >= 3.10 `uname -msr`
1. Update system packages: `apt-get update && apt-get upgrade -y`
1. Install Docker: <br>`curl -fsSL https://get.docker.com -o get-docker.sh`<br>
`sh get-docker.sh`
1. Install Docker Compose: <br>
`sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`<br>
`sudo chmod +x /usr/local/bin/docker-compose`
1. Ensure Docker Compose installed properly: `which docker-compose` should return a path to the executable.
1. Make sure git is installed; usually already installed in most DO droplets: `apt-get install git -y`
1. Change directory: `cd /srv`
1. Clone the HospitalRun fork repository: git clone git@github.com:Medic-NG/hospitalrun-frontend.git




### Configuration ###

