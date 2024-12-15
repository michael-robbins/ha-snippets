Just a collection of Home Assistant (HA) bits and bobs.

## Automations
[Tesla EV Charging off Solar Excess](blueprints/tesla_ev_solar_excess_charging.yaml)

Charge your Tesla completely offline via local connections to your PV inverter and your Tesla via Bluetooth. No Tesla API or internet connection required!

To set this up, we assume you've already:
* Setup [TeslaBleHttpProxy](https://github.com/wimaha/TeslaBleHttpProxy) and have it connected to the car (you can manually run commands via eg. `curl`)
* Ensure [ha-average](https://github.com/Limych/ha-average) is installed

## Snippets
[Tesla EV REST Sensors](snippets/tesla_ev_rest_sensors.yaml)

A set of rest sensors that rely on [TeslaBleHttpProxy](https://github.com/wimaha/TeslaBleHttpProxy)
