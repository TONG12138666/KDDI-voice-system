# KDDI-voice-system

启动的程序：

语音转文字：
roslaunch robot_voice iat_publish.launch
按space开始录音，按space结束录音。
ctrl＋c结束

文字转语音：
roslaunch robot_voice tts_subscribe.launch
重新发布话题，打开新终端：
rostopic list(可选)
rostopic pub /tts_text （tab补全）

注：可以修改台词。
缺点:1.语音转文字有时会出错，错了之后容易卡住。
    2.程序设计的像念稿子的一样，不能做到真正的互动，有思路以后会改进（或许）。
    3.没添加上语言模型，懒得搞了。
