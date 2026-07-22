# DGX Hackathon Journal

VLA Navigation 的单页开发历程：从 NVIDIA Isaac 仿真、InternVLA 快速导航、Step3-VL 多视角语义慢规划，到 ROS 2 / Nav2 与 Unitree Go2 的本地具身智能体控制闭环。

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
