# ffmpeg-hw-win32
ffmpeg 3.0  
gcc 5.3.0  
--enable-nvenc              nvidia_video_sdk_6.0.1  
--enable-libmfx             Intel(R)_Media_SDK_2016.0.1   
--enable-libfdk-aac         0.1.4  
--enable-libspeex           1.2rc1  
--enable-libx264            1:148.20150725  
--enable-libopenh264        1.5.0  
--enable-libx265            1.8  
--enable-libopus            1.1.2  
--enable-libmp3lame         3.99.5  
--enable-libkvazaar         0.8.2
 ```
 ./configure --prefix=/home/aliang/FFmpeg/x86_64 --enable-small --disable-debug --disable-doc --arch=x86_64 --cc='ccache x86_64-w64-mingw32-gcc' --cross-prefix=x86_64-w64-mingw32- --enable-cross-compile --target-os=mingw32 --enable-libfdk-aac --enable-libmp3lame --enable-libopus --enable-libspeex --enable-libx264 --enable-libx265 --enable-libmfx --enable-nvenc --enable-libopenh264 --enable-libkvazaar --enable-gpl --enable-nonfree
```
![img]

## Usage

(Windows path)

`git clone https://github.com/dansandland/ffmpeg-hw-win32.git && cd ffmpeg-hw-win32\x86_64\bin`

`ffmpeg -y -i sample.mp4 -vcodec nvenc -pix_fmt nv12 -f mp4 sample-out-nvenc.mp4`

[img]:https://raw.githubusercontent.com/illuspas/ffmpeg-hw-win32/master/h264-encoders.png
