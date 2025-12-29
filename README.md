# solar-teg-generator
Documentation for a solar powered generator that uses the suns rays to produce energy with thermoelectric generators (TEGs)

**Overview**
This project is to create a small solar powered generator that focuses sunlight to create heat, then used TEGs to transform that heat into energy.
TEGs are known to be *not that efficient* when compared to typical generators, so this project is not meant to break any records; It is merely for proof of concept.

Research into renuable energy is always important. Finding new ways to create power helps to save our planet, and make it easier for people to afford things in life. 
This project likely won't be breaking any record, but every little bit of research put into power generation brings us closer to better solutions to what we use today.

I've see TEGs be used to make energy, and solar focusing for heating, but I have never seen them used together. I'm curious why it isn't anywhere to be found (although I assume its due to its likely innefficiency).
I'll be measuring and documenting the output, so we shall see if this is the generator of the future or garage junk!

**How It Works**

This solar generator is shaped like a miniature Parabolic Troughs, which have a curved reflective part that reflects a large majority of sun that hits it into the object that the curve is centered around. 
They are a **complex parabolic** shape, which is important in order to reflect the material onto the center object on a wide range of angles
[Watch this video for a explaination of Complex vs normal parabolas] (https://www.google.com/search?q=complex+parabolic+generator+youtube&safe=active&sca_esv=0a4d36ace9aedeff&rlz=1C1GCPZ_en&ei=5A5SaeizKai0ptQP7JC4mAQ&ved=0ahUKEwjotYPeheKRAxUomokEHWwIDkMQ4dUDCBE&uact=5&oq=complex+parabolic+generator+youtube&gs_lp=Egxnd3Mtd2l6LXNlcnAiI2NvbXBsZXggcGFyYWJvbGljIGdlbmVyYXRvciB5b3V0dWJlMgoQIRigARjDBBgKSKc9UPMGWKA7cAF4AZABAJgBwgOgAb44qgELMS4zLjExLjEwLjG4AQPIAQD4AQGYAgagAr8JwgIKEAAYsAMY1gQYR8ICCBAAGIAEGKIEwgIIEAAYogQYiQXCAgUQABjvBcICBhAAGAcYHsICCxAAGIAEGJECGIoFwgIIECEYoAEYwwSYAwCIBgGQBgiSBwcxLjIuMS4yoAeAZLIHBzAuMi4xLjK4B7cJwgcFMS40LjHIBw6ACAA&sclient=gws-wiz-serp#fpstate=ive&vld=cid:8bdcefe4,vid:8zlAI32MSsQ,st:0 )

This redirected sunlight *should* heat the TEGs a good some of degrees
TEGs have two sides to them, the hot side  and the cold side
The temperature difference between these two sides is what determines the output energy of the TEG
To increase this temperature difference, we have the sun heating the one side, but we also want to keep the cold side cold
To do this, I'll add a heatsink with a fan (that will be powered by the generator itself)
The heatsink+fan will lower the temperature of the cold side and create more energy overall

The positive from the TEGs (which are connected in series) then goes to a blocking diode (to prevent discharge back from the Boost converter after)
This does slightly reduce output power, but is necessary for the safety of the project.

Then the positive goes to the in+ of the Boost Converter.
This turns the fluctuating energy that comes from the TEGs and turns it into a constant 5V (or 0V)
This constant voltage is necessary for using it to charge something, like a battery or phone

Coming out of the Boost Converter, I may introduce a Ammeter to measure the current of the power coming out. Then I'll record different observations based on this

The wiring then is split into two different circuits, one that connects to a USB-Micro cord to charge a power bank, then the other goes to power the fans in the heatsinks.

<img width="4328" height="2000" alt="unnamed" src="https://github.com/user-attachments/assets/da10b175-4023-4d16-bd95-096501e31887" />
Here is a **rough** drawing of the layout, but I'll do a CAD for the official 3d model later.


**Timeline**
If I get funding, I'll order parts within the week and then get working once they arrive.
The build itself will likely only take one or two long work days (~12-20h)
The majority of the time will have to be spent fixing it. 
There will likely be many overlooked issues, or broken parts
Then there will just be waiting around for new parts to arrive to keep working

After finalizing the design, I'll record data over a week or two and compile it for analysis.

**Risks & Safety**
There is, of course, the normal risks with tools and materials

Beyond that, the risks really depend on if this project works well.
The metal bar collecting heat will be dangerous to touch, if it actually ends up catching a good amount of heat
there is always the risk of electricution, but in this project, not as much because its never connected to wall outlets, so the only risk is when the TEGs output a strong amount.

