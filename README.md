# MSI-MAG-B560M-MORTAR-i7-10700
## 配置

macOS Big Sur 11.5.1 + OpenCore 0.7.1

| 组件 | 名称                                            |
| ---- | ----------------------------------------------- |
| CPU  | i7 10700                                        |
| 主板 | 微星 B560M 迫击炮 （MSI MAG-B560M-MORTAR-WIFI） |
| 显卡 | 蓝宝石 RX460 4GB 超白金版 + intel UHD 630       |
| 机型 | iMac 20,1                                       |

- [x] 睡眠唤醒
- [x] 核显驱动
- [x] 双硬解
- [x] CPU 变频

其他不完美的地方有

- 没有更换免驱的无线网卡，所以隔空投送、接力无法使用
- 自带的 intel AX210 网卡恰巧不在 itlwm 的驱动支持范围内
- 朋友手上没有 Type-C 设备，所以 USB 定制少了个 Type-C
- 另外 USB 定制有一个 USB2.0 口也无法工作，不过问题不大

## 细节

使用 OpenCore 0.7.1 

![](imgs/15155239.png) 

安装最新版本的 macOS Big Sur 11.5.1

![](imgs/Snipaste_2021-07-31_08-59-31.png) 

Hackintool 里面各项参数识别均正常，切完全支持 VDA 解码器：

![](imgs/Snipaste_2021-07-31_09-01-54.png) 

值得一提的是居然在图形显卡里面可以看到两个显卡，印象中双显卡是 MBP 专属的：

![](imgs/Snipaste_2021-07-31_09-02-46.png) 

因为驱动了核显，所以双硬解也都正常的：

![](imgs/Snipaste_2021-07-31_09-22-46.png) 

CPU 变频正常，也可以正常检测到核显的频率：

![](imgs/Snipaste_2021-08-01_00-28-25.png) 

GeekBench5 CPU 的多核跑分有点意外，超过 10 代 i9 了：

![](imgs/Snipaste_2021-08-01_00-43-35.png) 

AMD RX460 的跑分：

![](imgs/Snipaste_2021-08-01_00-44-08.png) 

Intel UHD630 的跑分：

![](imgs/Snipaste_2021-08-01_00-44-32.png) 

可以看出来 RX460 大概是核显的 4 倍性能左右，所以带 4k 的话，独显还是很有必要的。

另外各项传感器也均正常的： 

![](imgs/Snipaste_2021-08-01_15-15-56.png) 

 
