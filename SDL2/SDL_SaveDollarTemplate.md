# SDL_SaveDollarTemplate

Save a currently loaded Dollar Gesture template.

## Header File

Defined in [SDL_gesture.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gesture.h)

## Syntax

```c
int SDL_SaveDollarTemplate(SDL_GestureID gestureId,SDL_RWops *dst);
```

## Function Parameters

|                                |               |                                      |
| ------------------------------ | ------------- | ------------------------------------ |
| [SDL_GestureID](SDL_GestureID) | **gestureId** | a gesture id.                        |
| [SDL_RWops](SDL_RWops) *       | **dst**       | a [SDL_RWops](SDL_RWops) to save to. |

## Return Value

(int) Returns 1 on success or 0 on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_LoadDollarTemplates](SDL_LoadDollarTemplates)
- [SDL_SaveAllDollarTemplates](SDL_SaveAllDollarTemplates)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGesture](CategoryGesture)

