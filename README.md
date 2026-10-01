# Try-on Arena

多参考图虚拟试穿（Multi-Reference Virtual Try-On）的定性对比画廊。

给定同一张 source 人物图与若干件服装/配饰参考图及一条编辑指令，横向对比各开源/闭源模型的推理输出。

- 样本：15 例（`sample_index` 00005–00019，持续补充中）
- 参评模型：qwen-image-2.1、qwen-image-edit-2511、flux2-klein-base-9b、flux2-klein-base-4b、firered-image-edit-1.1
- 榜单：质量分、耗时、以及质量 × 耗时的散点分布

## 访问

<https://myosotisino.github.io/MR-VTON/>

## 说明

- 这是一个**只读**的静态快照，页面内不提供任何编辑入口，内容不可被访问者修改。
- 为控制体积，`assets/` 下的图片是面向 Web 投递的**缩小重压副本**（长边 900px，WebP），不是原始分辨率文件；页面中标注的分辨率描述的是模型那次推理的真实输出尺寸。
- 提示词为数据集 `caption.txt` 原文，未做改写。
- 本仓库仅托管展示用静态文件，不含数据集、权重与推理代码。
