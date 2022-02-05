# Escalator Controller using PIR , Buzzer , SPI LCD Screen

A C System that controls the number of people on an Escalator using a PIR Sensor , Buzzer and a screen to print the number of individuals on the Escalator . 

![Layout](https://github.com/TitiLouati/C-RaspberryPi-Project-Pi-Alarme/blob/main/Pi-Alarme-Raspi-project/LCDRaspi.png)

# Exmaple

The project Consists of three modes : 

## Detection of Person entering the escalator

the Detection of person will be done through a PIR Sensor that will be installed in the Gate of the escalator . 

## Printing the number of Person on the Escalator
 When someone gets on the escalator, the number of people will increase and will be printed on the screen.
 Each person have 10 seconds on the escaltor then he gets off and the number will decrease.

## turn on the Buzze take picture and sent it per email

if more than 10 people are on the escaltor. The buzzer will be turned on to alert that the number of people allowed is exceded. and a picture of the people that get on after the buzzer will be taken and sent per email to the user. The email address can be changed from sendrichtig.c file in the sonprocessSendemail function.


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

