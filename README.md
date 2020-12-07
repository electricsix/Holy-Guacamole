# Holy-Guacamole
Optimises usage of battery storage with Octopus Agile + Victron Multiplus &amp; Venus GX

Python script running on Raspberry Pi collects system info from Venus GX via MQTT & Agile tariff pricing from Octopus API. A desired SOC for each 30 minute time slot is then determined and the battery charged or allowed to charge based on the actual SOC relative to target.


Using the tariff data, there are also auxiliary outputs to run high load consumers such as electric heating & immersion at ideal times.

Temperature sensors are collated from around the house (via remote ESP8266 modules with DHT11 sensors) and amalgamated to act as a distributed thermostat. Heating is then switched according to distance from target temp and price.


User input file

All user inputs are captured in the HG-User-Inputs.py file

