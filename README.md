# ESPHome Xiaomi Device Configuration #
This is the configuration for my Xiaomi temperature and humidity devices being collected to Home Assistant using ESPHome. You need to have some secrets in your ESPHome `secrets.yaml` file or import the secrets from your Home Assistant `secrets.yaml`.

## Importing secerts from Home Assistant into ESPHome
Add the below line to the `secrets.yaml` file in the `esphome` subdirectory of the `/config` directory for Home Assistant.

```
# pull in from home assistant
<<: !include ../secrets.yaml
```

## Required secrets
* `wifi_ssid`
* `wifi_password`
* `esphome_ota_password`
* `esphome_api_encryption_key`
