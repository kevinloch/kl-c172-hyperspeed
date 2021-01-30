# kl-c172-hyperspeed
Cessna 172 (g1000) Hyperspeed Mod for MSFS 2020

## About
This package modifies the default C712 (g1000) aircraft in MSFS 2020 to allow it to acheive the maximum speed and altitude supported by the sim.  While this started as an experiment to explore the limits of the sim considerable effort has been put into making it stable and flyable over a wide range of conditions.  Below 3000 RPM it flys much like the default C172.  Above 3000 RPM engine performance increases dramatically, even exceeding 50,000 RPM at high altitudes and speeds.  This cartoonishly high RPM is the source of the extra thrust needed to achieve airspeeds as high as 2700 KTAS and altitude of 275,000 feet.  Maximum speed varies with altitude and weather.  At sea level and clear skies airspeeds of 1800 KTAS are achievable, with about 1400 KTAS in thick clouds.  Maximum airspeed increases with altitude by 30,000 feet the simulator max of 2700 KTAS is achievable.  While turning speed is normal at typical C172 speeds, it turns very slowly at extremely high speeds.   This mod is obviously made for entertainment purposes only and should never be used for real world training of any kind.

## Installation
Copy the `kl-aircraft-c172` folder inside the zip file to your MSFS Community folder.   If you want to revert back to the default C172, just remove `kl-aircraft-c172` from the MSFS Community folder.

## Important Notes
This mod requires the 'Modern' flight model and 'Disable Crashes' (set automatically when you enable developer mode in the sim).  In the 'Classic' flight model the aircraft is uncontrolable at high speeds.   If 'Disable Crashes' mode is not set you can easily overstress the aircraft and end the flight.  Ignoring the maximum speeds for flap extension is one of the reasons for this but also general aircraft stress limits.  I will look at eliminating the 'Disable Crashes' requirement in future versions.

## Normal Flight Envelope Operation
The hyperspeed modded C172 should behave vrey much like the default aircraft under normal C172 airspeeds and altitudes <b>IF you keep the engine RPM under 3000</b>.  

A few things are different however even in the low speed/altitude realm:
- Keep RPM around 2500 to remain in normal C172 flight conditions.  Do not allow RPM to exceed 3000 or you will quickly enter hyperspeed conditions.   If you do accidentially go faster than you want, extend flaps (regardless of airspeed) and idle throttle until you get below 3000 RPM.
- Mixture is set to 'Auto'.  If you have a controller bound to the mixture axis it will only control 'run' and 'cutoff', it will not adjust mixture.   This was necessary to support high altitudes.
- The fuselage and Landing gear drag coefficients have been set very low to support high speeds.  These drag settings have been added to the flaps drag so that when flaps are fully deployed it will have the same total drag as the stock C172.  When flaps are up the drag is very low which affects airspeed/acceleration at a given RPM as well as how it slows when the engine is at idle.  Since most slow/slowing flight is done with flaps at leat partially extended this feels like a reasonable compromise.
- Fuel flow rate is set to zero.  When the engine is running at hyperspeed RPM it would draw an enormous quantity of fuel, draining the C172 tanks in a few seconds.  While the fuel tank capacity could be set arbitrarily large this extra weight had very undesirable taxi and flying characteristics, even after setting max gross weight to account for the added fuel.

## Hyperspeed/Hyperaltitude Operation
Above 3000 RPM the engine has a physically impossible self-reinforcing power curve limited only by propeler drag which is a function of airspeed and altitude.  At very high altitudes this means you cannot idle the engine just by closing the throttle.   You must use drag (from flap extension) to slow the aircraft down so RPM can drop.  Descending will also help as the denser air will help slow the prop.

Tips for hyper speed and/or altitude operation
- For maximum performance takeoffs set elevator trim to -20% before takeoff.  Retract flaps once airborne and elevator trim gradually to -80% as max speed is attained.  You can also takeoff like you normally would in a C172 if you keep RPM to 2500 and accelerate to faster speeds once airborne.
- To slow down: set throttle to idle and extend flaps.  More flaps will create more drag and slow faster
- For maximum deceleration: set throttle to idle, extend flaps, and set mixture to 'cutoff'.  Descending to a lower altitude also helps.
- For intermediate speed cruising such as flying alongside an airliner, extend flaps 10 or 20 degrees and adjust throttle for desired airspeed.  At these middle flaps settings airspeed can be controlled reasonably well in the 300-600 knot range.
- Above about 60,000 feet altitude extend flaps or you will automatically accelerate to max airspeed regardless of throttle setting.  Mixture cutoff may occasionally be required under these conditions.
- For turns at very high speeds, bank 90 degrees in the direction of the turn and pull back on the stick VERY slightly.  Too much elevator is counterproductive and has the unexpected side effect of increasing airspeed, even beyond the normal limits for a given altitude.  Adjust bank angle for desired vertical speed.
- Slowing down will allow for tighter turns
- The default autopilot mode of 'ROLL/PITCH' is very helpful for fast trim adjustments if you have a key or controller button bound to autopilot engage/disengage.  Aim the pitch close to the desired attitude and briefely engage autopilot and release the controls.  Disengage autopilot a few seconds later after it has adjusted the pitch.  You can do this several times as the aircraft accelerates to quickly get trim in a usable range. 
