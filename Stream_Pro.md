# Multiple PC

Goto [Google Cloud Shell](https://shell.cloud.google.com/cloudshell/open?page=editor&shellonly=true&show=terminal&authuser=1)

## Github Repo Download (1st Time Only):

```bash
git clone https://github.com/jahidrdpschool/google-shell-live.git
```


## Try running a command now:

```bash
docker kill $(docker ps -q)
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
clear
echo "Downloading the Docker Image"
docker run -p 8080:80 -e RESOLUTION=1400x720 -d dorowu/ubuntu-desktop-lxde-vnc
clear
echo ""
echo "Access Link: https://localhost:8080"
echo ""
```

```bash
chmod +x pc-cloud-shell/multiple-pc.sh
./pc-cloud-shell/multiple-pc.sh
```