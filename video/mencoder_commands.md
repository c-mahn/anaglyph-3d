# Commands for processing Video from 3D side-by-side to 3D anaglyphic

## Processing left/right side-by-side Video into 1920x1080 anaglyphic 3D
mencoder -vf stereo3d=sbsl:arcd,dsize=1920:1080,scale "input.mp4" -o "output.mp4" -oac pcm -ovc x264

## Processing top/bottom side-by-side Video into 1920x1080 anaglyphic 3D
mencoder -vf stereo3d=abl:arcd,dsize=1920:1080,scale "input.mp4" -o "output.mp4" -oac pcm -ovc x264 
