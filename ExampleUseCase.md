# Introduction #
This page describes how jProTest can be used to perform Static Tests of Amateur Rocket Motors.

# Details #

In amateur rocketry, one builds motors for their rockets and then needs to characterize the thrust behavior of the motors.  This is done by performing static tests of the motors, recording the thrust as the motor burns.

|<img width='200' height='180' src='http://www.falkowski.net/images/bathroomscaletest_01.jpg'><table><thead><th><img width='240' height='180' src='http://www.falkowski.net/images/bathroomscaletest_02.jpg'></th></thead><tbody></tbody></table>

There are a variety of different systems that have been used to characterize the motor's thrust-time curve, ranging from a <a href='http://www.nakka-rocketry.net/static.html#Thrustometer'>grocery scale</a>, a scale coupled with a <a href='http://www.nakka-rocketry.net/static.html#Thrustograph'>mechanical graphing apparatus</a>, or more precise digital systems.  A simple example of a digital system uses a <a href='http://www.jamesyawn.net/electronicstand/bathscale/index.html'>digital bathroom scale's load cell</a> to convert the thrust into a voltage, then use a data acquisition system to convert the analog voltage to digital data that can be saved onto a computer:<br>
<br>
<table><thead><th><img width='200' height='180' src='http://www.falkowski.net/images/fourcomponentsfront.gif'></th></thead><tbody></tbody></table>

jProTest can be used in the simple digital scale system, but further simplifies the system by replacing the conventional DAQ hardware/software as follows.  A <a href='http://code.google.com/p/jprotest/wiki/HowToBuildVCO'>VCO circuit</a> should be built (less than $5) that converts the bathroom scale's voltage output to an audio signal.  The signal then can be recorded through a computer's sound card, or even by a digital audio recorder.  The audio file can then be processed by jProtest, which extracts the frequency of the signal vs. time, and allows calibration of the frequency back to the motor's thrust.<br>
<br>
Special recognition should be given to <a href='http://www.jamesyawn.net'>James Yawn</a> for his idea to use a digital bathroom scale for static tests and for the pictures of his equipment, to <a href='http://www.nakka-rocketry.net'>Richard Nakka</a> for his pioneering contributions, and to Paul Rehm