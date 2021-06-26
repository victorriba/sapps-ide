apt update

apt install curl build-essential python3 nano make gcc pkg-config libx11-dev libxkbfile-dev libsecret-1-0 sudo

curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh

sudo bash nodesource_setup.sh

sudo apt install nodejs

curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -

echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt update && sudo apt install yarn

yarn theia start /home/apps --hostname 0.0.0.0 --port 8080

nano ~/.bashrc


