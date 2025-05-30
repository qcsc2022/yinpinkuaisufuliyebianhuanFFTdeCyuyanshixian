# 音频快速傅里叶变换（FFT）的C语言实现

## 简介

本仓库提供了一个用于音频快速傅里叶变换（FFT）的C语言实现，该实现可以计算柱状频谱的幅值。资源文件中包含两个C代码文件和一个PCM资源文件。通过该实现，您可以对音频数据进行512点的FFT变换，并获取各个频率下的幅值，从而用于显示柱状频谱。

## 资源文件说明

### 1. `fft.c`
该文件包含了快速傅里叶变换（FFT）的C语言实现代码。通过调用该代码，您可以对输入的音频数据进行FFT变换，并获取各个频率下的幅值。

### 2. `main.c`
该文件是主程序，用于读取PCM数据并调用`fft.c`中的FFT函数进行变换。变换后的结果可以直接用于显示柱状频谱。

### 3. `440.pcm`
这是一个16位单声道的PCM数据文件，采样率为44100Hz。该文件包含了一个低频正弦波的音频数据，可以用于测试FFT变换的效果。

## 使用方法

1. **编译代码**：
   将`fft.c`和`main.c`文件放在同一目录下，使用C编译器进行编译。例如，使用GCC编译器：
   ```bash
   gcc -o fft_demo main.c fft.c
   ```

2. **运行程序**：
   编译成功后，运行生成的可执行文件：
   ```bash
   ./fft_demo
   ```

3. **查看结果**：
   程序将读取`440.pcm`文件中的512个采样点，并进行FFT变换。变换后的结果将输出各个频率下的幅值，您可以根据这些幅值来绘制柱状频谱。

## 注意事项

- 本实现仅支持512点的FFT变换，如果需要处理其他长度的数据，请自行修改代码。
- 输入的PCM数据必须是16位单声道格式，采样率应为44100Hz。
- 变换后的结果可以直接用于显示柱状频谱，您可以根据需要进行进一步的处理或可视化。

## 贡献

如果您有任何改进建议或发现了代码中的问题，欢迎提交Issue或Pull Request。我们非常欢迎您的贡献！

## 许可证

本项目采用MIT许可证，详情请参阅`LICENSE`文件。

## 下载链接
[音频快速傅里叶变换FFT的C语言实现]() 

(备用: [备用下载](https://pan.baidu.com/s/1xPuScIWmn1TYR2J3yM85Aw?pwd=1234))

## 说明

该仓库仅用于学习交流，请勿用于商业用途。
