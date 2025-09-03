I was the principal engineer on a project in which I was in charge of starting a new carbon fiber tube pultrusion process so that the company could make our tubes in house instead of buying from a supplier.

![[Pasted image 20250814131543.png]]
- (general representation of the machine and process ^)

The scope of this ~3 year project was **massive** and the manufacturing process itself is highly temperamental and prone to failure and unplanned downtime.

# The Process 
At the risk of greatly over-simplifying, this process involves pulling carbon fibers soaked in heat-cured epoxy resin around a rod (mandrel) and into a heated tube (die). 

# The Problem
If any of the many variable of the process are amiss, the composite structure fuses the die and mandrel together and requires upwards of 3.5 tons of pulling force to separate. 

This was dangerous to both the machine and the operators, and frequently caused several days of downtime in my R&D activities.

# The Solution
![[Pasted image 20250814133120.png]]

## Burning Carbon Fiber For Science
When reverse engineering composites, one method used is to heat the specimen to the point that the epoxy matrix combusts and separates from the composite so that you can examine the orientation and type of reinforcement used.

This inspired my solution of designing an oven specific to our tooling that was capable of reaching the necessary temperatures

## Mechanical
I used an industrial power cabinet as the housing, and machined unistrut as the means for the operator to suspend the bound up tooling.

![[Pasted image 20250814134252.png]]

I also had to spec out an exhaust blower that was explosion proof (acetone is used liberally in pultrusion,) corrosion resistant, and could move enough air to keep the enclosure safe to touch without being insulated and while also not robbing the tooling of heat

![[Pasted image 20250814134814.png]]

## Electronics
For the electronics, I used off the shelf components
- PID controller for temperature control
- Flexible heater tape for wrapping the tooling
- Thermocouple wire for temperature feedback
- 3 Phase VFD for the exhaust blower
- Various safety components 
- Convenience outlets

![[Pasted image 20250814135146.png]]![[Pasted image 20250814135200.png]]![[Pasted image 20250814135755.png]]![[Pasted image 20250814135303.png]]

# Results 
Since putting the oven into service, our downtime was reduced by 50%, and the mechanical force required to separate the tooling was brough down from ~3.5 tons to < 1 ton, which was safely achievable. The oven has over 350 hours of run time since time of writing