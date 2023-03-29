# emuThreeDS
World's first Nintendo 3DS emulator for Apple devices based on Citra.

## Progress
Progress updates for sections within the port.

### Audio
![100%](https://progress-bar.dev/100?width=110)  
Audio support is complete.
- Removed cubeb
- Updated SoundTouch

### Common
![50%](https://progress-bar.dev/50?width=110)  
Common's `file_util.h/.cpp` will need to be rewritten to support iOS.

### Core
![50%](https://progress-bar.dev/50?width=110)  
Core support is basically complete but will require testing.
- Replaced `pthread_jit_write_np` with `mprotect`
  - This needs looking into as I've not used mprotect before
  
### Dedicated Room
![0%](https://progress-bar.dev/0?width=110)  
No changes have been made to dedicated room yet.

### Input Common
![25%](https://progress-bar.dev/25?width=110)  
Input Common will need to be rewritten to support iOS.
- Removed `input_common`
- Controllers should still be supported via SDL2

### Network
![0%](https://progress-bar.dev/0?width=110)  
No changes have been made to network yet.

### Video Core
![90%](https://progress-bar.dev/90?width=110)  
~~Video Core currently crashes on `vkCreateSemaphore` and will require more work.~~  
~~Video Core now crashes at rendering and is likely due to `window_info.render_surface` being null.~~  
Video core no longer crashes but will require testing after the filesystem rewrite.

### Web Service
![0%](https://progress-bar.dev/0?width=110)  
No changes have been made to web service yet.
