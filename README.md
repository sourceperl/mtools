# mtools
MQTT tools suite to manage data (MQTT to ThingSpeak, web data to MQTT...) for Raspberry Pi

Setup Mosquitto for a Raspberry Pi:

    curl -O http://repo.mosquitto.org/debian/mosquitto-repo.gpg.key
    sudo apt-key add mosquitto-repo.gpg.key
    rm mosquitto-repo.gpg.key
    cd /etc/apt/sources.list.d/
    sudo curl -O http://repo.mosquitto.org/debian/mosquitto-repo.list
    sudo apt-get update
    sudo apt-get install mosquitto mosquitto-clients

Setup Python :

    sudo pip install -r requirements.txt

Setup mtools :

    sudo cp home/pi/.mtools_config /home/pi/
    sudo cp -r usr/local/bin/* /usr/local/bin/

Setup config :

Update .mtools_config with API credentials (Pushbullet, Thingspeak...)

Setup supervisor :

    sudo apt-get install supervisor
    sudo cp etc/supervisor/conf.d/* /etc/supervisor/conf.d/
    sudo supervisorctl update

