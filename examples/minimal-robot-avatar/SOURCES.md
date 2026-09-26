# 案例图片来源与许可

检索日期：2026-09-26。人物姓名来自来源页面说明，非从照片推断。案例仅演示照片风格转换，不表示照片作者、照片中的人物或其所属机构认可本项目。

| 文件 | 来源与作者 | 来源页面标注的许可 | 本地版本与修改 |
| --- | --- | --- | --- |
| `einstein/reference.jpg` | [Albert Einstein Head](https://commons.wikimedia.org/wiki/File:Albert_Einstein_Head.jpg)，摄影 Orren Jack Turner；页面记录 PM_Poon、Dantadd 等后期修改者 | 美国公有领域：版权未续期；其他地区状态见来源页面，并非全球统一公有领域 | Wikimedia 提供的 960 px 宽缩略版；原始黑白照片 |
| `mae-jemison/reference.jpg` | [Mae Carol Jemison (cropped 2)](https://commons.wikimedia.org/wiki/File:Mae_Carol_Jemison_(cropped_2).jpg)，NASA，S92-40463 | 美国公有领域，NASA 政府作品；见来源页面 | Wikimedia 提供的 960 px 宽缩略版；源页面为已裁切版本 |
| `tuxedo-cat/reference.jpg` | [Bicolor tuxedo cat](https://commons.wikimedia.org/wiki/File:Bicolor_tuxedo_cat.jpg)，Charlottekit；GeeAlice 作色彩校正 | 作者发布为公有领域，页面声明全球适用 | 来源页面当前版本，1024 × 768；未在本地修改 |
| `corgi/reference.jpg` | [Pembroke Welsh Corgi](https://commons.wikimedia.org/wiki/File:Pembroke_Welsh_Corgi.jpg)，Marsiyanka | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) | Wikimedia 提供的 960 px 宽缩略版 |

## 生成结果

每组 `avatar.png` 均使用对应参考图，通过 Codex 内置图像生成工具进行 AI 风格化，生成了胶囊眼、无鼻嘴、简化色块和新背景；不是原始照片、手工矢量描摹或官方肖像。

- 完整生成提示词记录于各组 `prompt.md`；进行过一次定向修正的案例另有 `revision-prompt.md`。
- `corgi/avatar.png` 为 Marsiyanka 原照片的 AI 改编，保留署名与来源链接，改编贡献采用 [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) 分享。该许可仅适用于这组图片及其改编，不自动适用于整个仓库。
- 其他来源照片保持各自原有权利状态；AI 结果不能反过来改变原照片的权利状态。
- 示例没有采用本次对话中用户上传的私人照片。

## 新增彩色人物与第二轮宠物测试

| 文件 | 来源与作者 | 许可 | 修改 |
| --- | --- | --- | --- |
| `jay-chou/reference.jpg` | [Jay Chou in Shanghai 2023 (3)](https://commons.wikimedia.org/wiki/File:Jay_Chou_in_Shanghai_2023_(3).jpg)，Play大明星 视频画面，Nkon21 调整 | [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/) | 下载来源版本；`avatar.png` 为 AI 风格改编，简化五官、发型和服装，重新构图与配色背景 |
| `taylor-swift/reference.png` | [Taylor Swift at the 2023 MTV Video Music Awards 4](https://commons.wikimedia.org/wiki/File:Taylor_Swift_at_the_2023_MTV_Video_Music_Awards_4.png)，iHeartRadioCA | [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/) | Wikimedia 500 px 宽缩略图；`avatar.png` 为 AI 风格改编，简化五官、发型和服装，重新构图与配色背景 |

人物图片仅作风格转换测试，无任何代言含义。上述生成版本保留原照片署名、来源与许可说明。

`tuxedo-cat/avatar-v2.png` 重新以原始猫照片生成；`corgi/avatar-v2.png` 以本目录上一版 `avatar.png` 为编辑输入，修改裁切和延伸感；提示词见各自 `prompt-v2.md`。柯基第二版同样是 Marsiyanka 原照片的改编，改编贡献采用 CC BY-SA 3.0。猫第二版仍存在物种轮廓和倾角偏差，保留为未通过测试。
