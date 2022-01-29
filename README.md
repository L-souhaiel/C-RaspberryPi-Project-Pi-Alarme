# Escalator Controller using PIR , Buzzer , SPI LCD Screen

A C module to controll how much personare on an Escalator from accessing a PIR Sensor , Buzzer and a screen to print the number of person are on the Escalator . 

![Layout](https://github.com/TitiLouati/C-RaspberryPi-Project-Pi-Alarme/blob/main/Pi-Alarme-Raspi-project/LCDRaspi.png)

# Exmaple

The project Consists of three modes : 

## Detection of Person entering the escalator

the Detection of person will be done throw a PIR Sensor that will be installed in the Gate of the escalator . 

## Printing the number of Person on the Escalator
 
every person who enter in the escalator will increase the number of person on the escaltor and these will be printed on the screen . every entred person to the 

escaltor will have 10 second to go out from the second gate . that means that the number of person will be decreased of 1 every 10 second.

## turn on the Buzze take picture and sent it per email

if more than 10 person are on the escaltor . the application will turn on the buzzer to make alarme sound . A picture containg the people entred the escaltor after 

the 10 will be taked and sent per email to the user . the email address can be changed from sendrichtig.c file in the sonprocessSendemail function . 


# Dependencies

install GCC compiler by instaling : libc6-armel-cross libc6-dev-armel-cross binutils-arm-linux-gnueabi libncurses5-dev build-essential bison flex libssl-dev. 

# Installation 


to install this project follow those steps: 


```
git clone https://github.com/TitiLouati/C-RaspberryPi-Project-Pi-Alarme.git

```
Then : 


```
gcc -o main main.c tone.c tone.h sendrichtig.c sendrichtig.h gpio.h gpio.c -lpthread

```

