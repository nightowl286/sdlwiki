# SDL_UnmapGPUTransferBuffer

Unmaps a previously mapped transfer buffer.

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
void SDL_UnmapGPUTransferBuffer(
    SDL_GPUDevice *device,
    SDL_GPUTransferBuffer *transfer_buffer);
```

## Function Parameters

|                                                  |                     |                                      |
| ------------------------------------------------ | ------------------- | ------------------------------------ |
| [SDL_GPUDevice](SDL_GPUDevice) *                 | **device**          | a GPU context.                       |
| [SDL_GPUTransferBuffer](SDL_GPUTransferBuffer) * | **transfer_buffer** | a previously mapped transfer buffer. |

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGPU](CategoryGPU)

