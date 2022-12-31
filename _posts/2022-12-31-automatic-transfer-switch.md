# Automatic Transfer Switch

An [automatic transfer switch](https://www.eaton.com/us/en-us/products/low-voltage-power-distribution-control-systems/automatic-transfer-switches/automatic-transfer-switch-fundamentals.html) automatically connects a load to backup power if the primary source fails. In my case, the load is a garage freezer that draws power from either a solar battery or the main house power. The solar battery is a limited energy source so it sometimes shuts down to preserve power during periods of cloudy days. In that case I’d like the freezer to draw mains power while the solar battery recharges. When the battery returns to a sufficient level of charge the freezer should reconnect itself to the battery, and so the cycle continues.

A double-pole-double-throw relay coordinates this operation by making electrical contacts between the two circuits depending on whether the primary power source is energized. A simple 12-volt wall-wart signals the relay to connect primary power when energized. On the other hand, if primary power is lost the wall wart de-energizes the relay, which switches the load to backup power.

![automatic_transfer_switch.jpg](/assets/automatic_transfer_switch.jpg)

I’ve added some night lights to indicate whether the primary circuit is energized.

# Schematic

Note, I’m not an electrical engineer so please excuse the terrible circuit diagram.

![transfer-switch-schematic.jpg](/assets/transfer-switch-schematic.jpg)

# Bill of Materials

| Item | Notes |
| --- | --- |
| DPDT Relay | sourced from https://www.mcmaster.com/69585K66/ |
| 12V wall wart | re-purposed from my phidgets SBC, can be https://www.phidgets.com/?tier=3&catid=61&pcid=54&prodid=175 |
| steel electrical box | 4x4 box https://www.homedepot.com/p/4-in-42-cu-in-2-1-8-in-Deep-Square-Box-721711234EW-20R/202590849 |