# Connected-Environments
Hey Duncan, this is Haoming Wang(Axe). I'll introduce what I have learned and skills develped from the project plant monitor.

Here we go

Firstly, set up feather. I downloaded the Arduino IDE and plug in my Huzzah to a USB port.
Then I use the given code to connect the lab wifi CE-hub-student with Arduino, it works.
After that, I went to the libraries and downloaded the ezTime library, when I opened the serial monitor, real time data could appear!

On the workshop, you taught us how to solder by showing the process on the screen. Actually, it was my first time doing things like this, I studied marketing when I was an undergraduate, so basically I have no idea about how to solder objects by using machine and wire.

With the help of video and other classmates, I started to do it by myself. To be honest, it's not really hard and also interesting! 
But be careful!!! 
When the machine turned on, the temperature is around 400 celsius, a very high figure so that it can melted wire. And when finished soldering, we should put the solder head back to the rest place, then stand up to offer next student to use the machine, do not pass the solder head to others by hand directly!!

This is my masterpiece, I connected the stitches to the board, although it looks not really nice, but it is very stable! I'm satisfied as professors always said "learning through doing". People always feel excited when they learn something new!

![soldering](/pictures/soldering.jpg)

Several weeks ago I learned how to use MQTT Explorer on Steven's Web Architecture lecture, so it is not hard for me to connect our lab's MQTT server. So I connected the Arduino board to my computer and MQTT, the light on the board flash when I send 1 through student/CASA0014/plant/zczqhw8/inTopic, vice versa, the light turned off when I sent 0 to MQTT server.

![MQTT-inTopic](/pictures/MQTT-inTopic.jpg)

So basically I thought it is a simple mould of IoT(Internet of Things) as I can use computer to control the object's status!

![add resistance and DHT22](/pictures/add-resistance-and-DHT22.jpg)

Next stage, I added 4 electric resistance to the board, which are two 10Ω, one 100Ω and one 200Ω. When I inserted these to the board, I should put them in the right position of the board, cut the remaining wire and soldered them as well. DHT22 is the sensor that we use in this project, which could help us to detect the environment temperature and moisture around the plant.

![connect-two-boards](/pictures/connect-two-boards.jpg)

In setup stage, I have already setup the pin for the DHT sensor, start the wifi and set up the MQTT server. By copy the code step by step that you gave to us, I can watch the data of my plant through MQTT server, including temperature, humidity and moisture.

![MQTT-Explorer](/pictures/MQTT-Explorer.jpg)

On the last session, there were a lot of work to do. At first is inserting SD card in the laptop, and start Respberry Pi programme to write related information in it. I have tried several times, but it didn't work. Therefore, I asked you for helping. You told me I have tried several times, the computer has a kind of protection peculiarity, so I need to open terminal and type sudo nano with file path to delete the related messages so that I can access to type password again! In addition, I should use my own username instead of pi which is after ssh and before @, so that I can type my password to login in. Importantly, after writing information in SD card, we should insert this SD card in Raspberry Pi and plug in.

![Raspberry-Pi](/pictures/Raspberry-Pi.jpg)


