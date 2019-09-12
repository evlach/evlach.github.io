[Electrical and Electronic Engineering](http://www.man.ac.uk/engineering/electrical)   MSF Decoder Electrical and Electronic Engineering Third Year Individual Project April 2000 The design and implementation of the project was done by [Evangelos Vlachogiannis](mailto:ejunior@ejunior.8m.com) The project supervisor was [Chris J Hardy](mailto:chris.hardy@man.ac.uk)    

[Read/download the report, the software and the manual](http://ejunior.8m.com/cgi-bin/framed/1838/mywork/projects/bscreport/bscreport.html)

Objectives Of The Project Main objectives

<table border="0" width="100%" cellspacing="0" cellpadding="0">

<tbody>

<tr>

<td valign="baseline" width="42">![](http://ejunior.8m.com/cgi-bin/framed/1838/mywork/projects/index_files/blebul1a.gif)</td>

<td valign="top" width="100%">Build a receiver for the 60 KHz standard time transmission from Rugby</td>

</tr>

</tbody>

</table>

<table border="0" width="100%" cellspacing="0" cellpadding="0">

<tbody>

<tr>

<td valign="baseline" width="42">![](http://ejunior.8m.com/cgi-bin/framed/1838/mywork/projects/index_files/blebul1a.gif)</td>

<td valign="top" width="100%">Decode to generate time and date using TMS370 microcontroller</td>

</tr>

</tbody>

</table>

<table border="0" width="100%" cellspacing="0" cellpadding="0">

<tbody>

<tr>

<td valign="baseline" width="42">![](http://ejunior.8m.com/cgi-bin/framed/1838/mywork/projects/index_files/blebul1a.gif)</td>

<td valign="top" width="100%">Show the information on an appropriate display</td>

</tr>

</tbody>

</table>

Additional objectives

<table border="0" width="100%" cellspacing="0" cellpadding="0">

<tbody>

<tr>

<td valign="baseline" width="42">![](http://ejunior.8m.com/cgi-bin/framed/1838/mywork/projects/index_files/blebul1a.gif)</td>

<td valign="top" width="100%">Other clock functions</td>

</tr>

</tbody>

</table>

Hardware Description The equipment used in our project is the following :

> [TMS370 MICROCONTROLLER](http://www.ti.com/sc/docs/micro/products/370_info.htm), by [Texas Instruments](http://www.ti.com/sc/docs/micro/home.htm)
> 
> The Texas Instrument TMS370 microcontroller is based around an 8 bit CPU which supports register to register operations on the 256 byte register file for simple addressing modes and accumulator based operations for extended addressing modes. The instruction set is optimized for control and measurement applications. A family of devices is available with a range of: package sizes and numbers of pins; RAM, ROM and EEPROM sizes; and peripherals. The[range of peripherals](http://www.ti.com/sc/docs/micro/products/370_mods.htm) are Serial Peripheral Interface (SPI), Serial Communications Interface (SCI), A to D conversion, Timers, Programmable Digital I/O and Programmable Acquisition and Control Timer.
> 
> It operates at a speed of 20MHz clock input. 13 I/O ports of the TMS370 are used in the following way:
> 
> *   for communicating with the LCD.
> *   for receiving the output from the Receiver Module.
> *   for the error LED.

It is an alphanumeric LCD with two lines of 16 characters.The Liquid Crystal Display (LCD) Module Antenna EM2 Receiver Module, by [Galeon Systems Ltd](http://www.galsys.co.uk/galmodul.htm). The Antenna together with the Receiver Module provide us with a digital output corresponding to the transmitted time and date information. The receiver is operating at a fixed frequency of 60KHz which is the required frequency for reception of the [MSF](http://www.npl.co.uk/npl/ctm/msf.html)time service transmitted from Rugby. The signal received is converted to a digital output by the receiver module. and the appropriate software is required to decode this output. Software Description The TMS370 was programmed in C language. The code that was executed by the TMS370 perform the following tasks :

*   Initialization of the LCD.
*   Displaying the information on the LCD and updating the display every second.
*   Decode the signal received from the receiver module.
*   Use Prediction Code for the Time and Date Code.
*   Use Correction Code for correcting the Time and Date code and report if errors have been received.

The size of the code had to be limited for two reasons :

*   The memory of the TMS370 is limited.
*   The accomplishment of high execution speed.

Useful Links

*   [National Physical Laboratory in Rugby](http://www.npl.co.uk/npl/cetm/taf/msf60.html) (information about the MSF signal)
*   [ICMaster](http://icmaster.com/) (search machine for finding any IC in the WWW)
*   [Temic Semiconductors](http://www.temic-semi.de/) (U4224B radio controlled clock receiver IC)
*   [Farnell](http://www.farnell.com/) (Supplier)
*   [CPC](http://www.cpc.co.uk/) (Supplier)
*   [Maplins](http://www.maplin.co.uk/) (Antenna EM2 Receiver Module)
*   [C-MAC Frequency Products](http://www.cfpwww.com/CFP2/home_j/home.html) (60Khz Crystals)
