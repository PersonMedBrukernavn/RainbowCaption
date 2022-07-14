# RainbowCaption
A small program to make the window title bars do an RGB cycle.

## Usage
An icon is added to the system tray area. You'll figure out the rest.\
Note that not all windows are supported, and in spesific cases there will be some visual bugs.\
When the program is shut down the title bars will not revert to their original colours.\
NB: If you run two instances of the process at once, they will compete and the title bars will flash a bit!

## The How
In Windows 11 Build 22000 a new feature was added to the DWM API through `DwmSetWindowAttribute()`, `DWMWA_CAPTION_COLOR`.
By passing in a COLORREF value, you can set the colour of the caption, no matter what process owns the window or if it's active or not.

## System Requirements
- 16KB Free Disk Space
- 1MB RAM
- Caveman Technoligy™ CPU
- Windows 11 Build 2200 or Newer