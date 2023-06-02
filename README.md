# PID-Project-Drag-Racer
By Joshua and Nick

# Table Of Contents
* [The Plan](#The-Plan)
* [Schedule](#Schedule)
* [Materials Used](#Materials-Used)
* [Code](#Code)
* [Wiring Diagram](#Wiring-Diagram)
* [CAD](#CAD)
* [Reflection](#Reflection)

# The Plan
For this project we planned to make a car using PID to simulate cruise control. Our car design was heavily inspired by the drag racers form last year with the main difference being that we'd have a photointerrupter containing the wheel spokes as a way to track RPM. We'd add an encoder to help change motor speed and the PID setpoint and an H-Bridge to allow for better motor control. 

# Schedule
4/18-4/21
Finish CAD

4/24-4/29
Begin and finish fabricating
the physical assembly 

5/1-5/5
Finish Build
Begin Coding and Wiring
Finish wiring

5/8-5/12
Finish Coding
Tune PID

5/15-5/19
Tune PID

5/22-5/26
Begin and finish documentation

# Materials Used
<ul>
  <li>Acrylic</li>
  <li>ABS</li> 
  <li>Dowel Rod</li>
  <li>Encoder</li>
  <li>Arduino METRO</li>
  <li>Prototyping Shield</li>
  <li>Wires</li>
  <li>9V Battery Pack</li>
  <li>Batteries</li>
  <li>DC Motors</li>
  <li>Photointerrupter</li>
  <li>Screws</li>
  <li>Nuts</li>

# Code
### GitHub Code: 
[PID Cruise Control](https://github.com/nbednar2929/CircuitPython/blob/master/PID_Cruise_Control)

# The Process of Coding
The process of coding was a long one. Firsly Nick had to learn how to use adafruit_motor to create a motor using AIN1 and AIN2. He then added in an encoder which would determine setpoint with and without PID. He also added in a photointerrupter and incorporated some of the PID library. At one point Nick used an AI to generate some code because he was struggling with how to find RPM, but the AI code didn't make it into the final product since Mr.Helmstetter was able to help him figure out some of the RPM logic. Mr.Helmstetter also helped him add half second intervals between calculating PID and RPM since the two can't happen simultaneously, something Nick spent lots of time trying to get to work before learning about its impossiblitiy. Finally he added code which mapped the encoder to motor power if the encoder is moved in a positive direction. He then mapped the same thing incoporating PID when the encoder is moved in a negative direction.  
  
# Wiring Diagram
![PID Wiring Diagram](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/91289646/47f96ed1-2691-4050-9e69-50d1b6a7920e)

# CAD
### Onshape Document:
[Link To Onsahpe Document](https://cvilleschools.onshape.com/documents/8f5f39db37f2e0703270eff9/w/33023e7b24fce4fc84bd36dd/e/18443bddf7985a762db6eef0)

### Pictures
![Full thing](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/0df4b95c-a3e1-4327-9ccc-e9ec51acf320)

### Wheels
![Big wheel](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/2bbb251b-38d3-4085-83df-4301b831f2f4)

This collection of parts are fully 3-D printed! Used in tandem with the gears and the DC Motors to propel the car forward.
![Small wheels](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/4f03f83c-0f20-4800-8b88-10d253b9f837)

Wheels are made of acrylic. We used a dowery rod for the axle. The coasters (parts in pink) are used to keep the wheels from slanting
they were challanging to make due to the fact that the dowery rod has an unconventional size that had to be accomidated for.

### DC Motor, Gears, and Brackets
![DC](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/899338d7-f561-418d-af17-b26badcfd963)
![DC 2](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/4338db37-61f9-4956-9b24-7d33b60ecae7)

The gears are attached to the DC Motors, they are friction fit. Nick designed specialized 3-D Parts that keep the motors in place.

### Car Body
![Body](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/603f1cd5-2ab4-4c82-b97f-689d4e46f99d)

This piece has undergone many changes, mostly just adding new holes for the increasing roster of parts that we needed.
### Axle Holder
![Holy savior](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/758b952c-f8f8-447c-8c79-90c5b89f197b)

This little guy holds the back axle which makes sure that it can rotate properly

### Photointerupter Bracket
![Photo broto](https://github.com/jbleakl36/PID-Project-Drag-Racer/assets/112979207/77274ff6-117c-4737-afc9-909c6acce2d5)

This piece is designed to hold the photointerupter in place so it can detect the movement of the wheels thus allowing 
steady data to flow so that we can properly undergo PID tuning.

# Assembly/Construction of the Vehicle
 Assembly came rather fast in the development of our project. We first created a drawing containing all of our acryllic parts.
 After that was printed we exported every part that we wanted to be 3-D printed. Time passes and eventually we get our 3-D parts,
 it was always exciting when this happened because that mean't that we could advance further into the development of our project.
 The first major problem we had was the fact that our car body had no holes for the battery pack and the metro. So Nick proceded to
 drill in the holes that were missing from the final part (makes sure to always double check your drawing, hit the refresh button 
 while your at it!). Unfortunatly Nick drilled the holes in the wrong spots (for the metro specifically) so we eventually had to 
 re-print the car body as we also in tandem with the missing holes added more holes for more parts (Nick still did a good job on the 
 drilling despite the errors along the way). Next up were the wheels, now the front wheels used a dowel rod as the axle which when 
 creating coasters (the pink parts that surrond both wheels) Joshua struggled to find a good size (he initially didn't use a caliper because
 we planned to 3-D print the axle for a short while) until around the 5th attempt which proved successful. The gears and the the axle 
 in the back were at first unable to fully rotate, so we created the axle holder (the white part shown above) to hold said axle in place
 while rotation was at hand. Sometimes the coasters come loose which is an issue cause it makes the small wheels unwieldy. The gears had a hard
time turning properly even with the axle holder, eventually it loosened up and began to turn well.

# Reflection
This project got off to a great start. We immediately began to make plans on a simple PID car and we began making it in CAD. The process went well,
we had good communication with each other and did not waste much time. Make sure to have a plan from the very start as you can get a lot done early on.
This was our main fault with the project, we failed to have a concrete plan of what we were doing and as a result many missteps took place. Holes weren't
added, an encoder wasn't added, minor design faults took place, and the code took vastle more effor than it should've given we were ignorant to the PID
library we were given for the first month or so of the project. Nevertheless we both designed different parts for the CAD but we made sure to communicate 
to each other about what we were making. It's very important to have good communication with your partner, that is something you should at the very least strive for.
Another fault that took place was the prospect of both of us working on CAD. After we had finished all that was left was code and documentation. Nick took on the code 
which took astronomically longer than any documentation Joshua could have done. This often left Joshua with little to do and Nick left to his own devices.
As the clock runs down on the time left to work on this project Nick wishes he had left Joshua to do the CAD and started doing code from the beginning. He also wishes
he had done a little more research about PID through either online sources or past Engineering projects which would've given him a better perspective on how
he should approach coding.
















