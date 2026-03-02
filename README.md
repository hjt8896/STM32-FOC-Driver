# BLDC FOC Control System
基于 STM32 的无刷直流电机（BLDC）有感磁场定向控制（FOC）系统实现。

## 1. 项目简介
磁场定向控制也称FOC，是一种电机控制方法，本设计将使用FOC算法对一个BLDC进行矢量控制，在这种控制方式下，电机能够输出很高精度的力矩和位置。

## 2. 核心特性
### 算法架构：
<img width="829" height="374" alt="image" src="https://github.com/user-attachments/assets/fa362a84-aba0-43e0-8d3f-25b5438ef67b" />

### 闭环控制：
构建了基于编码器反馈与电流采样的转速/位置双闭环系统。

### 性能优化：
通过 PID 参数优化，显著降低了运行噪声与震动，提升系统稳定性。

### 硬件平台：
基于 STM32 系列单片机开发，包含完整的功率驱动与保护电路设计。

## 3. 技术栈
### 硬件：
STM32G431CBU6、MOSFET 驱动桥、AS5048A磁角度传感器、3510云台无刷电机。

### 软件：
C 语言、Keil、Matlab/Simulink、STM32CUBEMX。

### 算法：
FOC, Clark/Park Transform, PID Control.

## 4. 项目结构
/Hardware: 原理图与 PCB 设计文件。

/Firmware: 基于HAL库的 C 代码。

/Simulation: Simulink 模型文件。

/Docs: 详细的技术文档、测试波形图与实验数据（截选自作者本科毕业论文，仅用于技术交流）。



