[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
# <a name="top"></a>![BrewPi Remix Logo](https://raw.githubusercontent.com/brewpi-remix/brewpi-www-rmx/master/images/brewpi_logo.png)

# A BrewPi Remix Fork of Fuscus

Fuscus is the Latin name for the Brown Water-Python.  It is also the name
[Andrew Errington](https://github.com/andrewerrington) chose for this
native Python implementation of the BrewPi fermentation controller.  Why
did he choose it?  I forget but it's buried in the [original thread](https://www.homebrewtalk.com/threads/native-python-brewpi-controller.575724/) somewhere I'm sure.

The [original project](https://github.com/andrewerrington/fuscus) was forked
to BrewPi Remix in order to allow the use of a Raspberry Pi within that
ecosystem.  Andrew's repo has not been updated since November 18th, 2016;
it's fair to say he's done with what he wanted to do.

## Does it work?

Let me say I don't think using a Pi for critical temperature control is
a good idea.  Having said that, here is what Andrew shared originally:

> There are very good reasons for allocating a microcontroller to the
task of heating and cooling control.  The primary one being that they
are very reliable.  If the Raspberry Pi should crash the microcontroller
will continue to monitor and maintain the last set temperature.  If
the control is done by the Pi then it could crash and leave the heater
or cooler stuck on, which will ruin the fermentation.
>
> Despite the possible risks of failure this project re-implements
the Arduino control code (v0.2.11) in Python so that it can run natively on
the Pi.  The other BrewPi components will
talk to this Python code as if it were an Arduino, so they can be be used
unchanged.  Hardware that was connected to the Arduino, such as 1-wire
temperature sensors, an LCD, and relays for the heater and cooler are
connected to the Pi GPIO pins.

Does this mean BrewPi Remix supports Fuscus?  Not at this time (3/19/21)
but it obviously means I'm playing around with it.
