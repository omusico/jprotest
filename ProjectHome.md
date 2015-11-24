|jProTest is an open source data acquisition tool written entirely in Java.  It receives data through a soundcard, which alleviates the need for special A/D equipment.  In fact, you can record your data onto a digital audio recorder, download the audio files onto your PC, and then import the audio files into jProTest.|<img width='155' height='150' src='http://www.falkowski.net/images/monitor.jpg'></tbody></table>

<h2>Features ##
  * Reads wav audio format
  * Extracts Frequency vs. Time
  * Charts data in X-Y Scatter Plot
  * Curve Fit the data
  * Print chart
  * Save image of chart as jpg


## Main Panel ##
The Main Panel displays the data, after defining correlation between data and the audio signal's frequency:

> <img width='450' height='320' src='http://www.falkowski.net/images/MainWindow_01.JPG'></li></ul>


<h2>Chart Preferences ##
The Chart Preferences Panel provides the ability to turn on/off the data, the curve that is fit to the data, and cross hairs that follow the mouse when moving over the chart.  It also provides some control for how the curve is fit to the data, and how the audio signal is calibrated to the data:

> <img src='http://www.falkowski.net/images/ChartPreferences_01.JPG'></li></ul>

<h2>Example Use Case (Amateur Rocketry) ##
In amateur rocketry, one builds motors for their rockets and then needs to characterize the thrust behavior of the motors.  This is done by performing static tests of the motors, recording the thrust as the motor burns.

|<img width='200' height='180' src='http://www.falkowski.net/images/bathroomscaletest_01.jpg'><table><thead><th><img width='240' height='180' src='http://www.falkowski.net/images/bathroomscaletest_02.jpg'></th></thead><tbody></tbody></table>

There are a variety of different systems that have been used to characterize the motor's thrust-time curve, ranging from a <a href='http://www.nakka-rocketry.net/static.html#Thrustometer'>grocery scale</a>, a scale coupled with a <a href='http://www.nakka-rocketry.net/static.html#Thrustograph'>mechanical graphing apparatus</a>, or more precise digital systems.  A simple example of a digital system uses a <a href='http://www.jamesyawn.net/electronicstand/bathscale/index.html'>digital bathroom scale's load cell</a> to convert the thrust into a voltage, then use a data acquisition system to convert the analog voltage to digital data that can be saved onto a computer:<br>
<br>
<table><thead><th><img width='200' height='180' src='http://www.falkowski.net/images/fourcomponentsfront.gif'></th></thead><tbody></tbody></table>

jProTest can be used in the simple digital scale system, but further simplifies the system by replacing the conventional DAQ hardware/software as follows.  A <a href='http://code.google.com/p/jprotest/wiki/HowToBuildVCO'>VCO circuit</a> should be built (less than $5) that converts the bathroom scale's voltage output to an audio signal.  The signal then can be recorded through a computer's sound card, or even by a digital audio recorder.  The audio file can then be processed by jProtest, which extracts the frequency of the signal vs. time, and allows calibration of the frequency back to the motor's thrust.<br>
<br>
Special recognition should be given to <a href='http://www.jamesyawn.net'>James Yawn</a> for his idea to use a digital bathroom scale for static tests and for the pictures of his equipment, to <a href='http://www.nakka-rocketry.net'>Richard Nakka</a> for his pioneering contributions, and to Paul Rehmann, a friend who suggested using a VCO.