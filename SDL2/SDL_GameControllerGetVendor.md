# SDL_GameControllerGetVendor

Get the USB vendor ID of an opened controller, if available.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
Uint16 SDL_GameControllerGetVendor(SDL_GameController *gamecontroller);
```

## Function Parameters

|                                            |                    |                                      |
| ------------------------------------------ | ------------------ | ------------------------------------ |
| [SDL_GameController](SDL_GameController) * | **gamecontroller** | the game controller object to query. |

## Return Value

([Uint16](Uint16)) Return the USB vendor ID, or zero if unavailable.

## Remarks

If the vendor ID isn't available this function returns 0.

## Version

This function is available since SDL 2.0.6.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

