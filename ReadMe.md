# Flipper Zero Weather Station Chaos

This is a copy of the Weather Station application from the [Flipper
Zero](https://flipperzero.one/) version 0.74.2 source, written mostly by
*Skorpionm*.

*It's intended for me to play around with external ELF/FAP files for the
Flipper. And to try to reliably hijack weather station info.*

*For now, I removed all protocols, except for the Clas Ohlson E0139ST2
(36-672x) model (Nexus), because that's the only Weather Station I
have. And I changed the icon.*

## Installation/running

- Clone the flipperzero-firmware repository.
  ```
  $ git clone --recursive https://github.com/flipperdevices/flipperzero-firmware.git
  ```

- Clone this repository into: `./applications_user/weather_station_chaos`

- Compile the binary using: `./fbt fap_weather_station_chaos`

- After a succesful build, you should have:
  `./build/latest/.extapps/weather_station_chaos.fap`

- Open up the `qFlipper` application, find the
  `weather_station_chaos.fap` application and upload it to `SD Card`,
  `/apps/`, `/tools/`.

Now you should be able to run it on the Flipper, from the
`Applications`, `Tools` menu.
