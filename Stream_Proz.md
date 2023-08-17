# Multiple PC

Goto [Google Cloud Shell](https://shell.cloud.google.com/cloudshell/open?page=editor&shellonly=true&show=terminal&authuser=2)

## Github Repo Download (1st Time Only):

```bash
git clone https://github.com/jahidrdpschool/google-shell-live.git
```

## Download System File (1st Time Only):

```bash
wget https://files.jahid.eu.org/1:/MyDrive/noVNC/Google%20Shell/System%20Files/stream_proz.tar
```

## PC Kill:

```bash
docker kill $(docker ps -q)
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
clear
```

# PC Making:

```bash
docker load -i stream_proz.tar
docker run -p 8080:80 -e RESOLUTION=1400x720 -d stream_proz
clear
echo ""
echo "Access Link: https://localhost:8080"
echo ""
```

## Try running a command now:

```bash
chmod +x google-shell-live/multiple-pc.sh
./google-shell-live/multiple-pc.sh
```
