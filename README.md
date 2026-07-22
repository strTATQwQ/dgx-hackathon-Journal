# DGX Hackathon Journal

本项目回应「让 Agent 创作一切」：依托 NVIDIA DGX Spark，把多模态创作从文字与图像延伸到空间理解、导航计划和真实世界行动。页面记录了从 NVIDIA Isaac 仿真、InternVLA 快速决策、Step3-VL 多视角语义慢规划，到 ROS 2 / Nav2 与 Unitree Go2 本地具身智能体闭环的完整开发历程。

作品面向建筑火灾造成断电、室内通信中断的救援场景：当云端链路不可依赖时，由现场 DGX Spark 持续完成多模态环境理解与 Agent 决策。单机构型使用 Step3-VL 进行高实时性语义导航；双机构型由 Step 3.7 Flash 负责高层环境探测与任务规划，导航节点持续执行和反馈。D435 与四路环视相机补足 Go2 原生低位前摄的观察范围，原型供电则在 STM32 打样周期不足时采用逆变器方案完成。

## 在线阅读

[https://strtatqwq.github.io/dgx-hackathon-Journal/](https://strtatqwq.github.io/dgx-hackathon-Journal/)

## 页面内容

- 项目动机与工程原则
- 七阶段开发历程
- 快 / 慢双路径控制链
- Step3-VL 在多视角理解、目标落地和候选排序中的作用
- NVIDIA、阶跃星辰、ROS 2 / Nav2 技术栈
- DGX Spark 本地部署与大模型优化方案
- 多仓库开源策略与公开边界

这是一个无构建依赖的单静态页面，样式与交互均内嵌在 `index.html` 中。GitHub Actions 会在 `main` 分支更新后发布到 GitHub Pages。

## 本地预览

```bash
python -m http.server 8000
```

打开 `http://127.0.0.1:8000/`。

## 公开边界

仓库只包含文章、页面代码与部署配置，不包含实验结果、运行日志、数据集、模型权重、原始相机画面、内部地址、用户名、凭证或私有路径。

## License

[MIT](LICENSE)
