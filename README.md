
# ESP32-S3-PhotoPainter

- 中文wiki链接: https://www.waveshare.net/wiki/ESP32-S3-PhotoPainter
- Product English wiki link: https://www.waveshare.com/wiki/ESP32-S3-PhotoPainter

## Change log

### [1.1.0] 2025/12/20
- In Mode 3, the scoring mechanism has been deprecated, and voice control capability has been newly added, which supports triggering the entry/exit operations of carousel images via voice commands, while also enabling dynamic adjustment of carousel interval duration through voice instructions;
- Fixed the abnormal issue where the device continuously restarts due to failed acquisition of weather data after the completion of network provisioning;
- Fixed the data overflow issue occurring in the interval wake-up process under Mode 1, upgraded the data type of the interval duration parameter from uint32_t to uint64_t to mitigate the risk of timer value overflow;
- Expanded the storage cache capacity for TF card file names to 80 bytes to accommodate scenarios with longer file naming conventions;
- Fixed the display anomaly where the device screen presents a blank screen when the TF card image reading operation fails.

## 更新日志

### [1.1.0] 2025/12/20
- 模式 3 中废弃打分机制，新增语音控制能力，支持通过语音指令触发轮播图片的进入/退出操作，同时支持语音指令动态调整轮播间隔时长；
- 修复配网完成后，因天气数据获取失败导致设备持续重启的异常问题；
- 修复模式 1 下间隔唤醒流程中出现的数据溢出问题，将间隔时长参数的数据类型从 uint32_t 升级为 uint64_t，规避定时器数值溢出风险；
- 将 TF 卡文件名称存储缓存的容量扩容至 80 字节，适配更长的文件命名场景；
- 修复 TF 卡图片读取操作失败时，设备屏幕出现白屏的显示异常问题。