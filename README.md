# mtools
MQTT tools suite to manage data (MQTT to ThingSpeak, web data to MQTT...) for Raspberry Pi

Setup Mosquitto for a Raspberry Pi:

    curl -O http://repo.mosquitto.org/debian/mosquitto-repo.gpg.key
    sudo apt-key add mosquitto-repo.gpg.key
    rm mosquitto-repo.gpg.key
    cd /etc/apt/sources.list.d/
    sudo curl -O http://repo.mosquitto.org/debian/mosquitto-repo.list
    sudo apt-get update

Setup Python :

    sudo pip install -r requirements.txt
