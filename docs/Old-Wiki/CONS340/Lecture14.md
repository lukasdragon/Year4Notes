What is GPS?

GPS stands for Global Positioning System. It is a group of government
satellites made by the U.S. to provide accurate information on
global/geographical positioning and navigation accessible from anywhere
on the Earth.

History

How does it work?

Components

Space Segment - satellites

-   GPS uses 24 satellites (3 of them are extras and are not active)
    that complete their orbit every 12 hours. Their orbits are situated
    so that at any point on the Earth's surface there are always 5 to 8
    satellites above the horizon.

Control Segment - ground stations

-   We have a total of 5 ground-based control stations. The main one is
    the Falcon AFB Colorado Springs These ground stations control the
    satellites and "talk" to them.

User Segment - receivers

-   This component is referred to as the "user". often where we receive
    the information sent from the satellites. GPS receivers and other
    users who compute velocity, time, and position using the satellite
    signals. The resulting information is often used for navigational
    purposes.

So How Does It Work? Triangulation!

GPS is a ranging system that does triangulation. Because it is
triangulating, it requires reference systems in the form of satellites
that move at 4 km/s. 

1.  The user (receiver) listens and detects 1-way signals from several
    satellites. Each transmission is a coded signal containing
    information along with the time-of-transmission and the satellite
    position. Signals are usually sent continuously (it is always
    sending something).
2.  The user compares the time-of-arrival of the signal and the
    time-of-transmission.
3.  The difference in time (delta T) is multiplied by the speed of light
    to obtain the range (or distance).
4.  Every range from a satellite in space puts us in a sphere around the
    satellite of a certain radius. This radius is the range.
    Intersecting several of these spheres allows the user to determine
    its position. Accuracy can be increased by increasing the number of
    satellites, and subsequently increasing the number of spheres.

-   Three satellites place us at one of two potential location points.
    To fix a three-dimensional location using satellites, we need 4
    satellites to eliminate one of the points.

Note on Distance Measuring

Distance = Rate x Time. 

Rate is the speed of light (186,000 miles/second). Time is the time it
takes for a signal to travel from the satellite to the GPS receiver.

Remember: the entire system is dependent on Time!

Measuring time on a satellite is done by SV clocks. There are 2 cesium
and 2 rubidium clocks in each satellite (\$100,000-\$500,000 each lol!)

Measuring time at the GPS receiver does not need cesium or rubidium
clocks. Receiver clocks are similar to a quartz watch. There are always
errors between the satellite and receiver clocks, and that is Delta T!
This is another reason why 4 satellites are ideal: they are required to
solve x, y, z, and Delta T.

Signals

Usually, two L-band carriers are used to broadcast GPS signals in a
Carrier Phase GPS.

-   L1 uses 1575.42 MHz and is modulated using both C/A-code and P-Code.
    It contains navigational messages and SPS code signals
-   L2 on the other hand uses 1227.6 MHz, and only the P-Code is used to
    modulate it. While unsophisticated satellites track only L1 using
    simple correction models, both L1 and L2 are required to filter out
    ionospheric delay by calculating the difference between the carriers
    (L1-L2).

Different from Carrier Phase GPS, Code Phase GPS primarily bases itself
on C/A codes.

The C/A Code

C/A stands for coarse acquisition. A C/A code is a series of 1 MHz
pseudo-random noise (PRN) codes - series of binary numbers - that
repeats itself every 1 millisecond. 

The Almanac

The almanac is a collection of additional information broadcasted by a
satellite about all the other satellites. When the receiver system is
powered up, the almanac provides initial information the user can use to
see where the other satellites will be located as well as their
condition status. And because satellites are in a fixed orbit and are
thus their locations are easily predictable, an almanac can be valid for
months. However, despite sacrificing some accuracy in the presented
format, an almanac is still a large file that can take several minutes
(up to 12.5 minutes) to complete its transfer.

Time is Distance

If we are able to calculate the difference in time between code
transmission and arrival, by looking at the difference between the code
received and the code generated by the receiver, we can determine the
distance between the satellite and the receiver. The greater the
difference in time is, the greater the distance between the satellite
and the receiver.

So if you want to make it harder for an outsider to gather accurate
information from your satellites, the best way is to include noise (that
we can easily identify) into the codes. This can be done using special
encrypted chips.

GPS Errors

Sources of GPS Positional Error can include:

-   Noise is typically the case. This can lead to slight variations in
    the location data, and this can be used to assess the accuracy of
    the data. 
-   Bias
-   Blunders/mistakes - putting in the wrong coordinates into your
    recording system, user error.

 

Multi-Path Errors

Multi-path errors can occur because a satellite sends out radio waves in
all directions. Anything can happen to these signals before they reach
the GPS receiver.

-   Signals are not pervious or penetrable through all objects.
    Buildings, trees, walls, and mountains can prevent transmitted
    signals from reaching you.
-   Signals can get reflected off of certain objects, including water,
    buildings, metal walls, etc. As a result, any signal received from
    the GPS receiver around this area may contain inaccurate data.

How to Reduce Errors

-   Do it in an open area where the sky is not blocked.
-   Avoid places with materials that might prevent or disrupt the
    signals, including buildings and tall trees.
-   Take multiple measurements to check.
-   Have patience, because satellites are always moving. With time,
    non-visible satellites may come into view and allow you to gain
    better measurements.

GPS and GIS