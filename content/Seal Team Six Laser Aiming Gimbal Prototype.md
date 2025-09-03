
We were approached but DEVGRU's (formerly known as Seal Team Six) Explosive Ordinance Division with a vague problem statement: 

They needed a way to precisely aim a heavy laser payload with minimal backlash, no backdriving, and they provided some general information about size, shape, and center of gravity.

Unsurprisingly, attempts to get more information bore little fruit. 

So I got to work thinking of a solution. Most of our existing products were not capable of the loads this application implied, or would require too much force input from the user to be practical.

I've previously designed motorized gimbal stabilizers (one of which was for the design challenge that landed me my current job.) I was also aware of a relatively exotic gear drive, cycloid drives, frequently used in industrial robotic arms. Cycloid drives are characterized by their lack of backlash, non back drivability, and high gear reduction.

![cycloidal gearbox IMTS 2018 on Make a GIF](https://i.makeagif.com/media/4-02-2021/wBB-DW.gif)

If you haven't seen one before, the way they transmit torque is mesmerizing to watch. These drives get their desirable characteristics from the very specific geometry of the spinning rotor (or rotors, more often than not) and the fact that they are always in tangential contact with the rolling elements on the inside and outside of the rotor.

What I came up with was a 19:1 gear reduction cycloid drive cartridge, one for each axis of rotation, that was hand cranked rather than being drive by a motor- I personally have not seen this implemented in such a way before.

![[Pasted image 20250812143441.jpg]]
![[Pasted image 20250812143420.jpg]]
![[Pasted image 20250812143429.jpg]]

Luckily for me, designing the drive was a matter of deciding what my overall size constraints and general gear reduction target was, as well a few other parameters affecting engagement and efficiency and tolerancing.

![[Pasted image 20250812144740.png]]

Some much smarter people than I have created an equation that takes my parameters, and creates the trademark eccentric cycloid

![[Pasted image 20250812144936.png]]

While this proof of concept hypothetically checked the vague boxes we were given, it ultimately would have ended up being too heavy for a soldier to be packing around. That's just how it shakes out sometimes (shrugs.) Still a very interesting project to have been given the reigns to explore 


![[20250306_093603_1 1.mp4]]