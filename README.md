# AI-Denglijun
基于 Sovits 4.0 开发的 AI 邓丽君模型。

## 流程

1. 收集邓丽君歌曲 60+ 首，并过滤去重到 59 首。
2. 使用 [Spleeter](https://github.com/deezer/spleeter) 将歌曲的伴奏和人声分离。
3. 使用 [RX-7](https://www.izotope.com/en/learn/using-rx-7-for-music.html) 手动对人声去除混响，得到干声。
4. 使用 [Audio Slicer](https://github.com/openvpi/audio-slicer) 对干声进行切片，下限 5s，上限 15s。
5. 使用 [Sovits 4.0](https://github.com/svc-develop-team/so-vits-svc) 进行模型训练和推理。

## 效果示例

金缕衣（原唱：姚贝娜）：`/demo/金缕衣_au_329600.mp3` 。

## 免责声明

本作品仅作为学习、娱乐目的发布，可能造成的后果与使用的音声转换项目的作者、贡献者无关。本项目基于 AI 音色替换技术 (Sovits4.0)，所合成的演唱人声并非邓丽君本人。模型仅供学习交流使用，严禁商用，违者后果自负。

如有侵权请告知删除。
