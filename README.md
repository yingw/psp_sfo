# PSP SFO repo

PSP (Sony Playstation Portable) 镜像内的 SFO (System File Object)  文件。[结构定义](https://www.psdevwiki.com/psp/Param.sfo)

PARAM.SFO 文件的路径： 镜像内:\PSP_GAME\PARAM.SFO

原版镜像 - 采用 Redump (v20250329) 定义的 dat 镜像集合
汉化版 - 采用 [OldmanEmu](https://www.oldmantvg.net/) 整理的 PSP中文游戏ISO全集(官中+汉化) (v20250426)，iso + cso 格式，共计563个(但是有个别镜像存在问题)

汉化版中的 SFO，一部分和基础版本一致，一部分做了修改（主要是编辑了 Title）

## 汉化版镜像问题

| 镜像                                                                    | 问题                             |
| ----------------------------------------------------------------------- | -------------------------------- |
| PSPCH009 – G弦上的魔王[汉化Lavis版]                                     | EBOOT 格式                       |
| 初音 将全部的歌献给未来的你                                             | EBOOT 格式                       |
| AKB1 48与偶像恋爱的话在关岛[简][ACG汉化组](含特典映像UMD+DLC+特典主题)  | 有2个ISO， 2nd.iso 是 UMD 视频牒 |
| 初音未来 歌姬计划(繁)[浜咲学园汉化组].iso                               | iso 损坏                         |
| 初音之歌 铃音之声 C75(中)[未知].iso                                     | iso 损坏                         |
| 鬼哭街[简体中文][萌乃妹汉化组]                                          | EBOOT 格式                       |
| 黑白棋大战(中)[未知](注释汉化版).iso                                    | iso 损坏                         |
| 花吻2 重装豪华版(繁)[未知].iso                                          | Unicode 解码错误                 |
| 蓝色玫瑰 妖精和青眼的战士(简)[Play汉化组].iso                           | iso 损坏                         |
| 库特Wafter(简)[Wafter汉化组](修改版).iso                                | Unicode 解码错误                 |
| 梦幻之星2 携带版 无限(中)[无限之星汉化组](v0.2_β公测物品汉化先行版).iso | Unicode 解码错误                 |
| 这间活动室被不回家部占领了 学园夏日战争篇[简][CG汉化组]                 | 无法解压                         |

- Python 解析脚本 [py.dataformat.sfo](https://github.com/Jasily/py.dataformat.sfo)
- sfo 编辑工具 [SFO Editor](https://archive.org/details/sfoeditor.-7z)
- 用 Python 库 [pycdlib](https://clalancette.github.io/pycdlib) 提取
