# Elecom HUGE : setting fn buttons

## install:
- xbindkeys
- xautomation

## add to ~/.xbindkeysrc
```
#fn1 : add sound
"amixer -D pulse set Master 3%+ unmute"
   b:10

#fn2 : turn down the sound
"amixer -D pulse set Master 3%- unmute"
   b:11

#fn3 : click the middle mouse button
"xte 'mouseclick 2'"
   b:12 + Release
```

## reload the config file
```
killall xbindkeys
xbindkeys
```

## execute the command : autostart
```
xbindkeys_autostart
```
