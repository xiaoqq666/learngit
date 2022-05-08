# DynamicSketch

### 文件

- p4/dynamic_sketch_epoch.p4: 实现了epoch更新的模块（待更新）。
- p4/dynamic_sketch_sampling.p4:实现了 sampling的模块（上一个较稳定的版本）。
- p4/common:一些通用的p4文件。

### 更新日志

#### 2022/05/04

**p4文件更新**

- 拆分原先的register，将每个bucket 对应的epoch_num由额外的寄存器存储。
- 在report  flowkey 和bucket value 时，加入对当前bucket 是否发生epoch 变化的判断


