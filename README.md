# DISTCOMP-E1: Distributed Computing | Crawling NASA's Sun

## Affiliation

![fondo-web2-10A-ENES](https://user-images.githubusercontent.com/100146672/160222385-4576c60e-1005-4753-b34d-c5461658c11b.png)

A project by Alexis Hassiel Nuviedo Arriaga ([@nuviedo](https://github.com/nuviedo)) ([alexis.nuviedo@gmail.com](mailto:alexis.nuviedo@gmail.com)), as part of the first partial exam of the Distributed Computing 2022-2 class imparted at the [*Escuela Nacional de Estudios Superiores*, campus Morelia](https://www.enesmorelia.unam.mx/), [UNAM](https://www.unam.mx/), by Dr. [Victor de la Luz](https://github.com/itztli).

## Problem description

The problem resides in programming a crawler to obtain the latest image of the Sun according to NASA's SDO.

![](img/latest_1024_HMIIC.jpg)

The problem was solved by making use of the built-in time & subprocess libraries to use wget every X minutes, whereas X is defined in the attached update_time.conf file as an integer numeral, without spacing. Namely, the algorithm will, until stopped, read from said file to know it's next wait time, proceed to sleep it blindly, and then download the image with wget in silent mode.

A running demostration can be found in UNAM's [GICC](http://www.gicc.unam.mx/) frontend server at my personal directory, [http://www.gicc.unam.mx/anuviedo/](http://www.gicc.unam.mx/anuviedo/).

## Requirements
* UNIX Bash terminal for execution, with wget available, in a writeable directory.
* [Python 3.+](https://www.python.org/)

## Steps to reproduce

* Execute [nasa_crawler.py](nasa_crawler.py), preferably as a detached background process.
* Update update_time.conf with the desired amount of minutes to wait inbetween calls.
* Extract resulting .jpg from current working directory as needed. 


## References
[NASA's Solar Dynamics Observatory](https://sdo.gsfc.nasa.gov/)

