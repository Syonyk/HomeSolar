# Panel Calculations

## Inverter Sell Output
Making this somewhat more complex than usual, the inverters are capable of selling less current onto the grid than their output - and aren't just a basic grid tied inverter, in which case this is all easy.

The GS8048 is limited to 30A of grid interactive sell current, and the GS4048 is limited to 15A.  Combined, this is 45A of possible grid sell coming back from the shed.  Multiplying by the 1.25x factor used for panel calculations, this is 56.25A of calculated sell current.

## Grid Load Panel (house) *705.12(B)(2)(3)(b)*
The grid load panel on the house has a 200A busbar, and serves combined power generation and loads.

It is protected by a 150A main overcurrent protection device on the grid side.  The maximum sell current that may come back from the inverters is 56.25A.

As the grid side and sell side breakers are at opposite ends of the busbar, 705.12(B)(2)(3)(b) applies, allowing 120% the busbar ampacity.

150A (main OCPD) + 56.25A = 206.25A.  120% of the 200A busbar rating is 240A.

## Grid-Side Panel (shed)
The power shed grid-side panel is protected (at the house side) by a 125A OCPD.  The maximum sell current from the inverters (x1.25) is 56.25A.  The combined total of 181.25A is less than the busbar rating of 200A, meeting the requirement of 705.12(B)(2)(3)(a), with no restrictions on breaker locations.