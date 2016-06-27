# Multi-room home system

The goal is to create a system like SONOS or similar using free software.

One of the problems to be solved is to use mobile devices as source and control of the stream.
Currently Volumio is very good using a local repository of audio either in a NAS or another.
The problem comes when you want to use a system like spotify from a smartphone.
From Android, you can not streaming directly to Volumio or other lan output device. You need a bluetooth receiver.
Volumio implements Spotify Connect but requires premium.
It also implements AirPlay for iOS and works very well but is useful only for Apple devices.

Another problem is the Bluetooth connectivity. Currently there are many multiroom systems but only allow one connection via Bluetooth. By definition, bluetooth can not connect more than one device.
This is going to try to solve by creating a distributed system using bluetooth receivers Raspberry pi to be placed in each room and will serve both, player with Volumio and bluetooth receiver.

The idea is to get any device with Bluetooth can connect to the system and play in any room.

When a device is connected to a Raspberry Pi by bluetooth, this will create a streaming that will be sent to a controller and this will transmit it to the players in each room.

![](https://github.com/franco8765/multiroom-home-system/blob/master/Stream%20flow%20components.001.jpeg)

## Links
### Streaming

* https://volumio.org/forum/multi-room-audio-system-with-raspberry-icecast-and-volumio-t2569.html
* https://wiki.archlinux.org/index.php/Streaming_With_Icecast
* http://www.activasistemas.com/blog/2013/08/19/montate-tu-propio-servidor-de-musica-domestico-con-raspberry-pi-icecast2-y-mpd/
* http://darkice.org/
* http://icecast.org/ices/docs/ices-2.0.2/config.html
* https://bbs.archlinux.org/viewtopic.php?id=97598
* http://www.alsa-project.org/main/index.php/Asoundrc
* http://crysol.org/es/node/1063

### Volumio
* https://volumio.org/
* https://github.com/volumio/Volumio2/wiki/WebSockets-API-Reference
