# SDL_SemTryWait

See if a semaphore has a positive value and decrement it if it does.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mutex.h)

## Syntax

```c
int SDL_SemTryWait(SDL_sem * sem);
```

## Function Parameters

|                      |         |                           |
| -------------------- | ------- | ------------------------- |
| [SDL_sem](SDL_sem) * | **sem** | the semaphore to wait on. |

## Return Value

(int) Returns 0 if the wait succeeds,
[`SDL_MUTEX_TIMEDOUT`](SDL_MUTEX_TIMEDOUT) if the wait would block, or a
negative error code on failure; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

This function checks to see if the semaphore pointed to by `sem` has a
positive value and atomically decrements the semaphore value if it does. If
the semaphore doesn't have a positive value, the function immediately
returns [SDL_MUTEX_TIMEDOUT](SDL_MUTEX_TIMEDOUT).

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateSemaphore](SDL_CreateSemaphore)
- [SDL_DestroySemaphore](SDL_DestroySemaphore)
- [SDL_SemPost](SDL_SemPost)
- [SDL_SemValue](SDL_SemValue)
- [SDL_SemWait](SDL_SemWait)
- [SDL_SemWaitTimeout](SDL_SemWaitTimeout)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

