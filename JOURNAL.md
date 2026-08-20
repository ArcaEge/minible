## Did research and started laying out schematic
Aug 18 • 1h30

I started by deciding which nRF to use and spent some time comparing. Looking at the featureset, the nRF52833 seemed pretty good: built-in USB, no need to use an external LDO, and all of this:

<img width="887" height="949" alt="image" src="https://github.com/user-attachments/assets/ecb0703c-fe9a-4dbb-8b7f-4e68bf42227a" />

Looks like only the nRF52833 and nRF52840 have USB support and this is cheaper, so I'll be using this.

## Finished schematics
Aug 19 • 2h

Schematics are done! I've looked through and added LCSC part numbers too, will be using some of my own parts that I already have. The rest of the parts will be 0402 to save on space and cost.

<img width="1265" height="922" alt="image" src="https://github.com/user-attachments/assets/5adc51c0-db28-4418-bd5e-dbd560bc4b28" />

Did some cost optimising too, switching to 0402s here and there. The current price is around $13 but if I bought in bulk (1000 boards) it'd be down to ~$3.80 per board - so pretty decent.

## Finished PCB, after many iterations
Aug 19 • 9h

Initially made this, a somewhat compact but still not that dense board:

<img width="756" height="904" alt="image" src="https://github.com/user-attachments/assets/67f4616b-1e49-4b95-9089-5777f368def2" />

Then I decided I should make it as tiny as possible, because [this thing](https://github.com/Dieu-de-l-elec/AngstromIO-devboard) exists and I want to beat that. They made a 9x8.9mm devboard and I wanted to see if I could do better.

<img width="777" height="736" alt="image" src="https://github.com/user-attachments/assets/32b5668c-d967-40c9-8b88-df3f0764d898" />

The layout and routing took a while but it's finally done! I spent a bunch of time rearranging everything to squeeze things closer together and it ended up being 8.9x9.5mm. Half a millimetre more in height but we also have Bluetooth, USB data and a much more powerful processor :)

<img width="782" height="750" alt="image" src="https://github.com/user-attachments/assets/7f764a58-3713-45e7-913b-d9ecc341de6d" />

A lot of jank was involved to get here - just look at the antenna 1206 pad :)

## Polishing up + curvy traces
Aug 20 • 5h

Added curvy traces - they look really nice on the board! Also added some silkscreen wave patterns:

<img width="1406" height="927" alt="image" src="https://github.com/user-attachments/assets/1155a9b2-fadf-4148-b2b4-007b74ad603b" />

<img width="814" height="736" alt="image" src="https://github.com/user-attachments/assets/1a614ee6-a5e7-464d-bd19-254543b7b8d0" />

The pads also got rearranged a bit so they're larger, also I had to switch to larger vias to save cost. The board is done, it ended up being 8.9*9.5mm - there isn't enough area to pack things tighter and still have space for pads.

It really is quite tiny...

<img width="1198" height="857" alt="image" src="https://github.com/user-attachments/assets/da07daf1-723d-4a06-917e-b2cba6fbc706" />
