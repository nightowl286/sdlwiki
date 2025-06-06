# SDL_strchr

Search a string for the first instance of a specific byte.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
char * SDL_strchr(const char *str, int c);
```

## Function Parameters

|              |         |                                         |
| ------------ | ------- | --------------------------------------- |
| const char * | **str** | the string to search. Must not be NULL. |
| int          | **c**   | the byte value to search for.           |

## Return Value

(char *) Returns a pointer to the first instance of `c` in the string, or
NULL if not found.

## Remarks

The search ends once it finds the requested byte value, or a null
terminator byte to end the string.

Note that this looks for _bytes_, not _characters_, so you cannot match
against a Unicode codepoint > 255, regardless of character encoding.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

