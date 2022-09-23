Firstly many thanks to John Miles at http://www.ke5fx.com and the RSGB, without there opensource designs this project would not be possible because I have no idea what im doing with electronics.

On a more serious note.

Dont be an idiot. 
X-band transmittions are usually regulated so dont assume you can just do random shit with this.
Check your local radio regulators be that OFCOM or the FCC or whoever regulates radio spectrum usage in your area to check this is legal and to aquire the neccesary licenses if it is not. 

Messing around with radio tranmitters can genuinly interfere with lifesaving equipment(and more relevant to the x-band, military radar, weather radar, landing radar) and can land you in serious trouble.
In the uk for example, illegaly transmitting in this band(or any non IMS band) can land your with an unlimited fine and or prison time up to 2 years.

You have been warned. 


It is popular online to convert these oscillator in to DIY synthetic Aperture radar. 

Do not do this.

Many technical hobbies have remained relativly unregulated because most users of the technology are responsible users and are considerate of the impact of there hobbies on those around them around, I do not see a resonable and considerate use for a SAR in the hobby scene
As access to these advanced technologies become more accessible to amateur hobbyist we risk further regulation limiting what responsible users can do
due to the actions of irrisonsible users. TLDR; dont be an idiot, dont be a dick, dont make military radars. 

I take no responsability for any consequeses you may face as a result of your usage of these documents. Dont come crying to me if you get fined and have your radio equipment seized.

Rant over.

Construction:
All parts needed to build the driver circuit are contained with in the Parts list text file. 
In addition to these parts you will need to manufacture the pcb, this can be done by the multitude of pcb manufaturing companines, PCBWAY will do it for less than £10 shipped. 
Or if your brave you can whip out your feric cholride and gas mask and do it yourself.
You will also need a metal project box, this is critical as the circuit is incredibly sensitive to radio noise that will disturbe op-amps causing an unstead output signal from the YIG

Required Tools:
An ESD safe soldering iron is a must, you can either buy you or you can add a grounding lead to your standard iron, this is just a wire that connects the hot end to a conductive grounded surface
such as a radiator, tap, grounding plug(if you have them where your live) or if your desperate a big ol' metal stake in the ground.
Solder, get some decent solder, dont get the ali express special.
Flux, this can be in the solder or you can use a seperate paste, its important to remove excess flux with acetone, rubbing alchohol, etc. Most flux is slightly to very conductive and may short you 12v supply to your op-amps 

Recommended Tools:
A pcb holder is also nice but not nessecary.
A solder sucker is nice to have and works way better than solder wick in my experiance. If your getting one get the ones with the "enveloping tips" trust me its worth it.

Other recommendations.
Use dip sockets for your ICs, this will protect them from the heat during soldering  and allows you to change then out if the let the smoke out.
The IRF510 MOSFET's will get hot, I have included space for heat sinks, use them. No the case cant be ventilated, no i dont know if it will help given that its entirly enclosed 

Changes:(this is important)
although the original design calls for LM627 Op-amps im using OP27G's, I dont know why, I dont know if it was my idea, I dont know if it makes it work better.
The original design calls for a bunch of extra resistors to stabalise the V+, and V- lines, ive ignored about 80% of them as they are all duplicates and can be replaced with larger caps if the total capacity of all of them is infact needed.

Warnings:
The YIG can get very hot when operating near the limits of its range, as such its probably best to disipate this heat to the casing of the project box to ensure the longevity of your oscillator.

The YIG is dumb. it will happly eat up 30 Amp and let out the magic blue smoke. no more than 200mA should be passed through any of the yig driving or modulating coils, 
you can either be real careful and set your driving offsets using the inculuded pots and test points or more sensibly you can add a 
series 200mA fuse in series with the tuning lines to save your precious oscilattor if you do a dumb.

The Modulation Signal cannot be more than 1 Volt peak to peak. 

This is a relativly new project, there may well be errors everywhere.

Helpful stuff:
The tune line with alter the output frequency by about 5MHz up or down for every 1mA of current change
The Vcc line with draw about 80mA
Tuning coil impedance is nominaly at 15 Ohms
Modulation coil impedance is nominaly 0.5 Ohms
The oscilattion outpus about 15mW though some people say this is closer to 25mW, i dont have the test equipment needed to check 
