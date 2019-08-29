pvrtc-decompress

Copied & modified from https://github.com/tlozoot/decompress-pvrtc

Compile: 
gcc -std=c99 -o pvrtc-decompress decompress.c fortseige_pvr.c

Usage:
pvrtc-compress <input.pvr> <output.bmp> <width> <height> <is_2bpp|0|1>

Notes:
- input.pvr should be raw compressed texture, not PVR file with header
- This will auto flip output bmp vertically
- is_2bpp should be 0 for 4bpp, or 1 for 2bpp
