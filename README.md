raspKaku
========

Control your KAKU with Raspberry


=======================================================================================================================

These files make it possible that if you follow the tutorial that is on tweak blog about turning on and off lights 
with 433 mhz to use the new kaku (system). And I also added the possibility to send the adress instead of hardcoded.

Leave a comment i you change or add shizzle

:)

good luck, have fun


//personal comment

git clone git://git.drogon.net/wiringPi

cd wiringPi

./build

git clone https://github.com/chaanstra/raspKaku

in bijv kaku.cpp de juiste pin_out selecteren (staat standaard op 15)

cd raspKaku

g++ -o kaku kaku.cpp -I/usr/local/include -L/usr/local/lib -lwiringPi

Niet vergeten:
sudo nano /etc/init.d/domoticz.sh
/usr/bin/gpio export 18 out
