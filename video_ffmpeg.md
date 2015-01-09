# 编解码工具:FFmpeg

## 介绍

不是所有浏览器都支持统一格式，因此需要有一款编解码工具转换视频格式，方便开发。

FFmpeg是一套可以用来记录、转换数字音频、视频，并能将其转化为流的开源计算机程序。采用LGPL或GPL许可证。它提供了录制、转换以及流化音视频的完整解决方案。它包含了非常先进的音频/视频编解码库libavcodec，为了保证高可移植性和编解码质量，libavcodec里很多codec都是从头开发的。

FFmpeg在Linux平台下开发，但它同样也可以在其它操作系统环境中编译运行，包括Windows、Mac OS X等。这个项目最早由Fabrice Bellard发起，现在由Michael Niedermayer维护。许多FFmpeg的开发人员都来自MPlayer项目，而且当前FFmpeg也是放在MPlayer项目组的服务器上。项目的名称来自MPEG视频编码标准，前面的"FF"代表"Fast Forward"。

**官方网址：**www.ffmpeg.org


## 功能


多媒体视频处理工具FFmpeg有非常强大的功能包括视频采集功能、视频格式转换、视频抓图、给视频加水印等。

**视频采集功能**

ffmpeg视频采集功能非常强大，不仅可以采集视频采集卡或USB摄像头的图像，还可以进行屏幕录制，同时还支持以RTP方式将视频流传送给支持RTSP的流媒体服务器，支持直播应用。

**FFmpeg's Logo**

以进行屏幕录制，同时还支持以RTP方式将视频流传送给支持RTSP的流媒体服务器，支持直播应用。

**ffmpeg在Linux下的视频采集**

在Linux平台上，ffmpeg对V4L2的视频设备提供了很好的支持，如：
./ffmpeg -t 10 -f video4linux2 -s 176*144 -r 8 -i /dev/video0 -vcodec h263 -f rtp rtp://192.168.1.105:5060 > /tmp/ffmpeg.sdp

以上命令表示：采集10秒钟视频，对video4linux2视频设备进行采集，采集QCIF(176*144)的视频，每秒8帧，视频设备为/dev/video0，视频编码为h263，输出格式为RTP，后面定义了IP地址及端口，将该码流所对应的SDP文件重定向到/tmp/ffmpeg.sdp中，将此SDP文件上传到流媒体服务器就可以实现直播了。

**ffmpeg在windows下的视频采集**

在windows下关于ffmpeg视频采集的资料非常少，但是ffmpeg还是支持windows下视频采集的。ffmpeg支持windows下video for windows(VFW)设备的视频采集，不过VFW设备已经过时，正在被WDM的视频设备所取代，但是ffmpeg还没有支持WDM的计划，不过好像有将WDM转为VFW的工具，因此ffmpeg还是可以在windows下进行视频采集的。

**视频格式转换功能**

ffmpeg视频转换功能。视频格式转换，比如可以将多种视频格式转换为flv格式，可不是视频信号转换 。

ffmpeg可以轻易地实现多种视频格式之间的相互转换(wma,rm,avi,mod等)，例如可以将摄录下的视频avi等转成视频网站所采用的flv格式。

**视频截图功能**

对于选定的视频，截取指定时间的缩略图。视频抓图，获取静态图和动态图，不提倡抓gif文件;因为抓出的gif文件大而播放不流畅。

**给视频加水印功能**

使用ffmpeg 视频添加水印(logo)。