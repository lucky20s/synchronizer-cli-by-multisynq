# synchronizer-cli-by-multisynq

**Register here <a href="https://startsynqing.com/?ref=f91ab7-4wc069">startsynqing.com</a>**

**Prerequisites**
- Node.js v10 or higher
- Docker
- Synq key (Obtain From Their Discord Channel https://discord.gg/GseWHYVH)

**Let's Go!**
```
sudo apt update -y && sudo apt upgrade -y
```

**Install NodeJs**
```
apt get-install wget curl -y
```
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
```
```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```
```
nvm install --lts
```

**Install synchronizer-cli**
```
npm install -g synchronizer-cli
```

**Install Docker**
```
synchronize install-docker
```
*choose Y*

**Interactive configuration**
```
synchronize init
```
*follow the instruction*

**Running Node**
```
synchronize service
```
```
sudo cp ~/.synchronizer-cli/synchronizer-cli.service /etc/systemd/system/
```
```
sudo systemctl daemon-reload
```
```
sudo systemctl enable synchronizer-cli
```
```
sudo systemctl start synchronizer-cli
```
*wait 1-2 minutes*

**Setup Dashboard Service (Optional)**
```
synchronize service-web
```
```
sudo cp ~/.synchronizer-cli/synchronizer-cli-web.service /etc/systemd/system/
```
```
sudo systemctl daemon-reload
```
```
sudo systemctl enable synchronizer-cli-web
```
```
sudo systemctl start synchronizer-cli-web
```
**Log into your dashboard service:**
- visit your-ip:3000
- login using any-username and password you have created before


