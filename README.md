Just a collection of Home Assistant (HA) bits and bobs.

## Automations
[Tesla EV Charging off Solar Excess](blueprints/tesla_ev_solar_excess_charging.yaml)

Charge your Tesla completely offline via local connections to your PV inverter and your Tesla via Bluetooth. No Tesla API or internet connection required!

To set this up, we assume you've already:
* [REQUIRED] Setup [TeslaBleHttpProxy](https://github.com/wimaha/TeslaBleHttpProxy) and have it connected to the car (you can manually run commands via eg. `curl`)
* [RECOMMENDED] Install [ha-average](https://github.com/Limych/ha-average)
  * And configure a series of 'averages' over your import and export sensors
  * See [these snippets](snippets/tesla_ev_solar_averages.yaml) for examples
* [REQUIRED] The [following entities](snippets/tesla_ev_charging_required_entities.yaml) available to use by the automation
* [REQUIRED] These [REST Sensors, REST Command and entities](snippets/tesla_ev_rest_sensors.yaml) are available to use by the automation
* Import the blueprint into Home Assistant with this URL: `https://raw.githubusercontent.com/michael-robbins/ha-snippets/refs/heads/main/blueprints/tesla_ev_solar_excess_charging.yaml`
