# Homey-Luxtronik
This repository provides the source code for the Luxtronik app available to Homey users. The Wiki and Issue tracker for this project are also to be found here.

This app lets you add heatpumps to Homey from the following manufacturers:
- Alpha Innotec
- Siemens Novelan
- Roth
- Elco
- Buderus
- Nibe
- Wolf Heiztechnik
- Novelan

Neither of these manufacturers are connected to this project. Some images used in this project are owned by Alpha Innotec.

## About
This app is mostly based off of previous work like [Bouni/luxtronik](https://github.com/Bouni/luxtronik), [Bouni/python-luxtronik](https://github.com/Bouni/python-luxtronik) and [BenPru/Luxtronik](https://github.com/BenPru/luxtronik).

The app only support Luxtronik 2 / 2.1 controllers currently, but YMMV.
The following functionality is currently supported:
| **Values**                    | **Getable** | **Settable** | **Comment**                                  |
|-------------------------------|-------------|--------------|----------------------------------------------|
| **Total used Energy**         | Yes         |              | AFAIK this is heating energy                 |
| **Energy used for heating**   | Yes         |              | AFAIK this is heating energy                 |
| **Energy used for Water**     | Yes         |              | AFAIK this is heating energy                 |
| **Energy used for Pool**      | Yes         |              | AFAIK this is heating energy                 |
| **Outdoor Temperature**       | Yes         |              | This, obviously, requires an outdoor sensor  |
| **Room Temperature Current**  | Yes         |              | This currently required the RBE room display |
| **Room Temperature Set**      | Yes         |              | This currently required the RBE room display |
| **Temperatue of Hot Gas**     | Yes         |              |                                              |
| **Water Temperature Current** | Yes         |              |                                              |
| **Water Temperature Set**     | Yes         |              |                                              |
| **Source Temperature In**     | Yes         |              |                                              |
| **Source Temperature Out**    | Yes         |              |                                              |
| **System Temperature Suppy**  | Yes         |              |                                              |
| **System Temperature Return** | Yes         |              |                                              |
| **System Water Flow**         | Yes         |              |                                              |
| **General Operation Mode**    | Yes         |              | This depends on the type of Heatpump         |


## Workings
This app talks to the heatpump based on TCP-communication. You will need to add the heatpump manually (as it currently does not support any discovery methods). It then queries the heatpump on a schedule and updates the sensors accordingly.

## Examples
Currently, the most useful use cases I can think of are:
- Creating flows based on outdoor, room, or system temperatures
- Creating flows based on operation mode.

## Support me
[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/robinf)
