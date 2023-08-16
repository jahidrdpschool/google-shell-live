# Multiple noVNC

## Github Repo Download (1st Time Only):

  1. Open Google Cloud [Shell](https://shell.cloud.google.com/?hl=en_US&fromcloudshell=true&show=terminal&authuser=1).
  2. Run this command:
```bash
git clone https://github.com/jahidrdpschool/pc-cloud-shell.git
```

  ## Step 1: Launch the first novnc2

  1. Run this command:
      ```bash
      docker kill $(docker ps -q)
      docker rm $(docker ps -a -q)
      docker rmi $(docker images -q)
      clear
      docker run -p 8080:80 -e RESOLUTION=1400x720 -d dorowu/ubuntu-desktop-lxde-vnc
      clear
      echo ""
      echo "Access Link: https://localhost:8080"
      echo ""
      ```
  2. Wait for the container to start.
  3. Cloud Shell Click on "Access Link: [https://localhost:8080](https://shell.cloud.google.com/devshell/proxy?port=8080&environment_id=default&authuser=1)
  4. Close the Cloud Shell tab, but keep the novnc2 tab open.

  ## Step 2: Launch novnc2

  1. novnc2: Go to Google [Cloud Shell](https://shell.cloud.google.com/?hl=en_US&fromcloudshell=true&show=terminal&authuser=1) Tab.

  ## Step 3: Automate launching multiple novnc2
  1. novnc2: Open a new terminal in Google Cloud Shell.
  2. novnc2: Run this script:
      ```bash
      chmod +x pc-cloud-shell/multiple-pc.sh
      ```
      +
      ```bash
      ./pc-cloud-shell/multiple-pc.sh
      ```
  3. novnc2: Follow the prompts to enter the number of 2 PC you want to launch.
  4. novnc2: Cloud Shell Click on: "Access Link 1: [https://localhost:8001](https://shell.cloud.google.com/devshell/proxy?port=8001&environment_id=default&authuser=1)"
  5. Now Open Main Tab: [https://localhost:8002](https://shell.cloud.google.com/devshell/proxy?port=8002&environment_id=default&authuser=1)


  ## Step 4: Install OBS Studio
  1.
```bash
sudo apt update
 ```
