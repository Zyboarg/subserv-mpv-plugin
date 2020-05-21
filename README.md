# subserv-mpv-plugin for Windows 
Send subtitles displayed by mpv to your web-browser.

A plugin for https://mpv.io/
the mpv video player.

This plugin starts a webserver together with your instance of mpv, which will send displayed subtitles to your web-browser.
It was created for the purpose of studying the japanese language with the help of japanese subtitled anime.

More on the method here: http://learnjapaneseonline.info/2013/11/05/learn-japanese-through-anime/

With this plugin and the help of yomichan (https://foosoft.net/projects/yomichan/) it becomes simple to look up definitions and add cards to your anki-deck, while watching japanese subtitled anime in mpv.

![picture showcasing subserv coupled with yomichan](http://i65.tinypic.com/2ufbxqu.jpg)

# Installation:
to compile and install it basically run:
```
gcc -o ~/.config/mpv/scripts/subserv.so subserv.c -I . -shared -fPIC
```
mpvs 'client.h' needs to be included.
You can get it from https://raw.githubusercontent.com/mpv-player/mpv/master/libmpv/client.h
Just save it in the directory you are compiling it from.

To access the site, just go to 127.0.0.1:8080 (if you want to change the port, edit the port definition in the source).

If you have any questions, feel free to send them to kyouko@channel.moe
