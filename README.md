Basic Setup:

    Make sure to install nmap: sudo apt-get install net-tools nmap
    And to run: sudo setcap cap_net_raw,cap_net_admin,cap_net_bind_service+eip /usr/bin/nmap


Mosquitto:

    Install mosquitto MQTT: `sudo apt-get install mosquitto mosquitto-clients`

    Set up Mosquitto user/pwd: `sudo mosquitto_passwd -c /etc/mosquitto/passwd YOUR_DESIRED_MQTT_USER_HERE`

    Change `/etc/mosquitto/conf.d/default.conf` to have these contents:
        allow_anonymous false

        password_file /etc/mosquitto/passwd
        port YOUR_DESIRED_PORT_HERE

    Restart Mosquitto: `sudo systemctl restart mosquitto`

    Don't forget to fill our your MQTT configs in mqtt.yaml
