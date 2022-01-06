# TiArt
## 项目作者
shonge
## 项目进展
开发中
## 项目介绍
基于TiDB-Dashboard Key-visual实现绘画功能
## 项目背景&动机
Just for fun
## 项目设计
1. 固定 keyvisual bucket range，确保 asixY 稳定
2. 缩短 asixX 统计间隔至 10s
3. 将读取图片转成黑白并分割成128*128块
4. 根据每个块平均灰度生成读取次数n，按每块y值生成row id
5. 从左至右每10秒逐列读取rowid数据n次
6. 1280秒后绘画完成
