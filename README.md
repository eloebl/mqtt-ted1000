# mqtt-ted1000
Reads the TED1000 via the specified USB port and posts it to MQTT

INSTALL
=================
```
sudo apt-get install git python-pip

sudo pip install setuptools
sudo pip install setproctitle
sudo pop install paho-mqtt

mkdir /etc/mqtt-ted1000/
git clone git://github.com/mloebl/mqtt-ted1000.git /usr/local/mqtt-ted1000/
cp /usr/local/mqtt-ted1000/mqtt-ted1000.cfg.example /etc/mqtt-ted1000/mqtt-ted1000.cfg
cp /usr/local/mqtt-ted1000/mqtt-ted1000.init /etc/init.d/mqtt-ted1000
pdate-rc.d mqtt-ted1000 defaults
cp /usr/local/mqtt-ted1000p/mqtt-ted1000.default /etc/default/mqtt-ted1000
```
Edit /etc/default/mqttted1000 and /etc/mqtt-ted1000/mqtt-ted1000.cfg to suit"
`/etc/init.d/mqtt-ted1000 start`
