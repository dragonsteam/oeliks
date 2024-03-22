# oeliks

A Free advertising platform

## setup a server for development and testing

- update and upgrade ` sudo apt update && sudo apt upgrade -y`
- install docker engine
- add you user to docker group `sudo gpasswd -a $USER docker`
- restart current session (restart if it doesn't work)
- setup github action-runner
- clone `oeliks-server` repository
- setup docker secrets file (SECRET_KEY and TELEGRAM_BOT_TOKEN are required)
- configure ufw (allow ssh, http and https ports)
- install nginx
- copy everything inside `nginx.conf` file here into `/etc/nginx/sites-available` directory
  and link it in `/etc/nginx/sites-enabled` folder
- finally get ssl sertificate using certbot
