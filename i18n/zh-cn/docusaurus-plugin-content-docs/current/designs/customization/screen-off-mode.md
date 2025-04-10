---
sidebar_label: 息屏模式
---

# 息屏模式

![Design](/img/design/2ffc61f3-4d57-4570-9500-071e80ffea80.png)

> ① 表盘 A
>
> ② 表盘 A 的息屏模式
>
> ③ 表盘 B
>
> ④ 表盘 B 的息屏模式

息屏模式允许设备在息屏状态下呈现时间等关键信息，让用户无需抬腕即可快速获取重要资讯。
息屏模式的显示类型主要分为以下两类：

- 跟随当前表盘：使用当前所使用表盘所附带的息屏样式。
- 自行选择设置的表盘：用户根据个人喜好与使用习惯，自主挑选任意息屏表盘样式 。

息屏表盘的制作规范请参考：[息屏表盘制作规范](../../watchface/specification.md#息屏模式)

## 设计原则

- 指针与数字：避免显示秒针或数字秒。
- 时间刻度：可保留时间刻度，以提高时间辨识度。
- 资源一致性：确保指针和数字切图与正常表盘的尺寸一致。
- 息屏模式与正常显示模式切换：尽量减少不同模式下元素的位置差异，避免切换时出现位移。
- 其他数据：除了时间外，根据需要展示其他数据（如步数、日期、天气、电量、心率等）。

## 数字类表盘处理方法

![Design](/img/design/e8c952bb-e60e-4903-8705-684eeaf6f235.png)

> ① 表盘
>
> ② 息屏模式案例 A
>
> ③ 息屏模式案例 B

- 时间数字：
  - 建议使用描边线型设计，线条建议使用纯白色（#FFFFFF）。
  - 秒数字：请移除秒的数字。
- 表盘背景：请移除渐变背景色及大面积背景图，将表盘背景设定为纯黑色（#000000）。
- 颜色规范：避免使用过多颜色，并确保 RGB 颜色值中至少有一种大于等于 128（例如 R:0，G:0，B:128）。若使用灰色，请确保 RGB 颜色值大于 153（例如 R:160，G:160，B:160）。
- 大面积元素：当 RGB 中有一个值超过 182（例如 R:120，G:120，B:200）时，建议将大面积元素改为线宽 6px 以下的描边。对于 RGB 值均低于 182 的元素，目前则不需要考虑。

![Design](/img/design/05dffa12-3cd7-45a0-b120-e545ec4bb073.png)

> ① 错误案例：RGB 颜色值均低于 128
>
> ② 正确案例
>
> ③ 错误案例：存在大面积元素，其 RGB 有一个值超过 182
>
> ④ 正确案例
