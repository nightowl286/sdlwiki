# SDL_HINT_JOYSTICK_WHEEL_DEVICES_EXCLUDED

A variable containing a list of devices that are not wheel style controllers.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_JOYSTICK_WHEEL_DEVICES_EXCLUDED "SDL_JOYSTICK_WHEEL_DEVICES_EXCLUDED"
```

## Remarks

This will override
[SDL_HINT_JOYSTICK_WHEEL_DEVICES](SDL_HINT_JOYSTICK_WHEEL_DEVICES) and the
built in device list.

The format of the string is a comma separated list of USB VID/PID pairs in
hexadecimal form, e.g.

`0xAAAA/0xBBBB,0xCCCC/0xDDDD`

The variable can also take the form of "@file", in which case the named
file will be loaded and interpreted as the value of the variable.

This hint can be set anytime.

## Version

This hint is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

