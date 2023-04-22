# home_assistant_solarbat
Automation examples for Home Assistant with Wallbox, Givenergy and Tesla

The code in ha_automations.yml can go into automations.yml and the code in ha_configuration.yml goes into configuration.yml

This will not work out of the box, at the very least you need to fill in the xxxxx with your device names/IDs

This uses:

- Wallbox integration
- GivTCP for Givenergy battery integration
- Tesla integration
- Solcast integration

The Octopus slot ON/OF automations are used to get the Tesla to charge during Octopus intelligent cheap slots while stopping the home battery discharging
The Wallbox automations are to charge the car from Solar when the home battery is full during the daytime
There is a cleanup for Wallbox to cancel stuff off if the car is aborted manually (e.g. unplugged)
There is an automation to update the solar forecast from Solcast twice a day, and then load the overnight home battery charge % based on next days forecast and your predicted usage.

Please use as an example only, create your own based on your devices and needs.
