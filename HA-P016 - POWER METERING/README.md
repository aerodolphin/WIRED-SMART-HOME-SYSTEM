# GOALS

Measure the power consumption using a EASTRON SDM120 device.

## Material Necessary

*   1x SDM 120
*   1x RS485 TLL
*   1x Nodemcu v3 ou Wemos D1

[LINK TO INFO.md](info.md)

```
sensor:
  - platform: mqtt
    state_topic: 'tele/sdm120/SENSOR'
    value_template: '{{ value_json["ENERGY"]["Voltage"] }}'
    name: 'Voltagem'
    unit_of_measurement: "V"
    icon: mdi:speedometer

  - platform: mqtt
    state_topic: 'tele/sdm120/SENSOR'
    value_template: '{{ value_json["ENERGY"]["Current"] }}'
    name: 'Corrente'
    unit_of_measurement: "A"
    icon: mdi:speedometer

  - platform: mqtt
    state_topic: 'tele/sdm120/SENSOR'
    value_template: '{{ value_json["ENERGY"]["ActivePower"] }}'
    name: "Potência (W)"
    unit_of_measurement: "W"
    icon: mdi:speedometer

  - platform: mqtt
    state_topic: 'tele/sdm120/SENSOR'
    value_template: '{{ value_json["ENERGY"]["ApparentPower"] }}'
    name: 'Active apparent power'
    unit_of_measurement: "VA"
    icon: mdi:speedometer

  - platform: mqtt
    state_topic: 'tele/sdm120/SENSOR'
    value_template: '{{ value_json["ENERGY"]["ReactivePower"] }}'
    name: 'Reactive apparent power'
    unit_of_measurement: "VAR"
    icon: mdi:speedometer

  - platform: mqtt
    state_topic: 'tele/sdm120/SENSOR'
    value_template: '{{ value_json["ENERGY"]["Factor"] }}'
    name: 'Factor Power'
    unit_of_measurement: ""
    icon: mdi:speedometer

  - platform: mqtt
    state_topic: 'tele/sdm120/SENSOR'
    value_template: '{{ value_json["ENERGY"]["Frequency"] }}'
    name: 'Frequencia'
    unit_of_measurement: "HZ"
    icon: mdi:speedometer
```

## \## THE WAY TO GO: SDM120 modbus RTU nodered

[https://community.home-assistant.io/t/no-response-from-modbus-slave-2-register-0/58943/33?u=aerodolphin](https://community.home-assistant.io/t/no-response-from-modbus-slave-2-register-0/58943/33?u=aerodolphin)
