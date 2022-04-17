# Home Assistant Setup

Make a copy of `.env.example` as `.env` and then fill in the blanks:

`HOME_ASSISTANT_CONFIG`: The directory path where your Home Assistant configuration is. By default it's set to the directory included with this repo.

`MOSQUITTO_CONF_PATH`: The directory path where your Mosquitto configuration is.  By default it's set to the directory included with this repo.

`MOSQUITTO_DATA_PATH`: The directory path where your Mosquitto data is stored.  By default it's set to the directory included with this repo.

`MOSQUITTO_LOG_PATH`:  The directory path where your Mosquitto logs would be stored.  By default it's set to the directory included with this repo.

`MOSQUITTO_PUID`: The UID belonging to the user running the Docker container

`MOSQUITTO_GUID`: The GID belonging to the user running the Docker container

`TIMEZONE`: Default to America/New_York

`ZWAVE_SESSION_SECRET`: A randomly generated alphanumeric string for the Z-Wave session