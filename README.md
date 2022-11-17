# nRF24L01-Nucleo
PROJECT SUMMARY :

   This system is designed for a Olive Picking Machine. Firstly , we are reading 12x analog variable like a potantiometer. They give us position information of steering wheel and beaters. After reading the values, we have 16x PWM output to control the lenght of machine , steering wheels, position of the beaters and the machine according to the trees. Secondly, we are choose using a RF remote controller to control the machine parts separately. In RC(Remote Controller), we are planing to send 2 digital signal in addition to the data package. One of is Overwrite Signal to make an overwrite for the values that comes from the machine parts and the other one is Voltage-Detect Signal for understanding if the RC is opened or not. Lastly, we recoded that when the tranciever part is starting to run in begining, the values and data packeges are coming randomly for a moment. Hence, We can put some delay but we are going to use 2 more digital signals on tranciever side for the same reasons with the RC part and to prevent random machine movements. As it is seen above, we are using analog pins , timer pins for pwm, SPI pins for RF Controller.To give one more little information for the machine, it consists of only electrical and hydraulical systems.
   
   How to Use : 
   
![image](https://user-images.githubusercontent.com/70060259/202440002-ebf6e4ef-6710-4a84-a548-7e4e312a3843.png)
   Here is the pinout of nucleo.
