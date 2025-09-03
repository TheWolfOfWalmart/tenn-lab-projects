Early in my career as a Product Development Engineer, I developed a system to perform vibration analysis on the carbon fiber tubes we used to make our tripods. Later on as I was tasked with starting our in-house tube manufacturing, this process became critical to my R&D activities and determining how the tubes I was making performed compared to the tubes we were buying.

#  The setup
![[Pasted image 20250819110921.png]]![[Pasted image 20250819111033.png]]

I designed a V-block fixture for the tube specimens, and a process for ensuring repeatability between setups.

I used a 3 DoF accelerometer affixed to the same point along the tube relative to the fixture.

# Making Waves
To test how the tubes responded to vibrations, I needed a controlled way to excite the tubes and ended up with two methods:

## The Ball Drop
![[Pasted image 20250819111531.png]]

The first and most simple method was to drop a mass from a controlled height. I used a ball bearing that was held in place by a pin, and the drop height was controlled using a 123 block for reference. The pin was pulled allowing the ball to fall and impact the tube with the same energy every time.

## Surface Transducer
![[Pasted image 20250819112131.png]]
Have you ever seen one of those devices that, when pressed against a surface (E.g. a wall, a box, a table etc...) turns that surface into a speaker?- Those are surface transducers. They are essentially speakers that vibrate surfaces directly, rather than using a diaphragm that modulates air pressure.

![[Pasted image 20250819112819.png]]

The transducer would be hooked up to an amplifier, which allowed me to vibrate the transducer at using any waveform of my choosing. This signal could come from a traditional waveform generator, or any 3.5mm audio output.

# Analyzing The Results 
The last piece of the puzzle was visualizing the results. I used an oscilloscope to read the output of the accelerometer. From there, I was able to quantify and compare natural frequency, impact force, resonant frequencies, and vibration dampening.
![[Pasted image 20250819113926.png]]
![[Pasted image 20250819113932.png]]![[Pasted image 20250819113936.png]]

In reality, vibrations are rarely one frequency. By applying a fast fourier transform in a spectral analyzer, I was able to break down any given impulse into it's frequency components

![[Pasted image 20250819114332.png]]
![[Pasted image 20250819114336.png]]
![[Pasted image 20250819114344.png]]

# Results
Because of this process, I was able to correlate the vibrational characteristics of our R&D carbon fiber tubes and lay the ground work for production, and the future development of vibration damping composite structures 