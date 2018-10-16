# NAS-VPN-Downloader-Automation-Pack
A collection of docker-compose scripts to facilitate download automation on docker compatible NAS systems

Includes things like [lidarr](https://github.com/lidarr/Lidarr), [radarr](https://github.com/Radarr/Radarr), [sonarr](https://github.com/Sonarr/Sonarr), and [nzbget](https://github.com/jshridha/docker-nzbgetvpn) / [transmission](https://github.com/haugene/docker-transmission-openvpn) running inside OpenVPN with sample configurations for [NewsHosting](https://newshosting.com/) and can be modified to work with other providers.

## How to use

Export the following vars (of course modify to your setup if needed):
    
    export PUID=0
    export PGID=1000
    export TZ="America/Chicago"
    export USERDIR="/shares/"


Then, for each container that you wish to run, navigate to the compose folder and modify the .yml file appropriately then run:

    docker-compose -f <THEFILENAME> up -d