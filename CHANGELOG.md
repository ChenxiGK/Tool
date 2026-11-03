# Changelog

## v1.2.0
- 采集默认改用 **DXGI Desktop Duplication**（`ddagrab` + `hwdownload`），GPU 侧合成，
  解决「推流时本机鼠标指针闪烁」问题；不支持或多屏副屏时自动回退 `gdigrab`。
- 新增采集方式下拉（auto / dxgi / gdi）与 DXGI 自动回退逻辑。

## v1.1.0
- 新增 **ONVIF Profile S 设备端**：WS-Discovery 自动发现 + Device/Media 标准服务 + JPEG 快照，
  NVR 可「一键添加」，频道列表显示缩略图。
- ONVIF WS-Discovery 绑定到专用网卡 IP；端口占用自动降级 80 → 8080 / 8081。

## v1.0.0
- 初始版本：ffmpeg + MediaMTX 内置 RTSP 服务，屏幕实时采集编码为 H.264 推流。
- 专用网卡绑定（静态 IP / 防火墙 / UAC 提权）、编码器自动探测（NVENC/QSV/AMF/x264）、
  连通性自检、托盘常驻、开机自启。
