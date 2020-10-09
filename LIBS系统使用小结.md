## LIBS系统使用小结

---

### 1 硬件

#### 1.1 激光器的开关

#### ![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008162800.png)

#### 1.2  光谱仪的开关

![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008162908.png)

#### 1.3 旋转实验台

![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008163321.png)

#### 1.4 延时器

![](https://gitee.com/lim-gitee/blog-image/raw/bdff1d81def2ab9f11c4c3f19125ba211b1b23c7/img/20201008164308.png)

##### 1.4.1

![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201009100531.png)

> 1 显示区
>
> > Delay灯亮
> >
> > SEC亮
>
> 2 触发区
>
> > EXIT亮：外触发，上升沿触发
>
> 3 通道选择
>
> > 输出线与通道选择对应
>
> 4 控制
>
> > 对1区域中的数字进行大小调节，调节的是1中正在闪的那位数字

---

### 2 软件

#### 2.1 $$GCD$$使用

![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008192817.png)

> 1. COM选择---COM3，点击connect
> 2. 运行控制中：地址选择1
> 3. 方向为remote
> 4. 速度为4.67mm/s
> 5. 行程一般100，循环为10N
> 6. 点击执行

#### 2.2 Avosoft使用

![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008193146.png)



![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008195834.png)



![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201009101757.png)

![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008195133.png)

 1. 预先检测，依次点击$$File——Excel——Merge0$$

    ![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201008200740.png)

    

    勾选Active表示将测量数据输出到Excel中

    > Continues模式下勾选此项则会导致一直将背景光谱输出，电脑可能死机
    >
    > 出现此种情况进入任务管理器结束Avosoft这个软件

    a）Single Column为不平均直接将每次结果输出

    b）Column per scan 表示平均多少次之后将结果输出到excel（一般选这个）

​	2 先测量背景噪声（点击start即可，默认测量即为Continuous），即为使用激光器激发时的噪声情况，当Measurements大于200时即可暂停

​	3 点击Dark（绿色圆形按钮）按钮保存所测得的背景噪声（步骤1、2目的是去除环境条件的干扰）

​	4 将测量模式改为L,B.I.S，点击Options——Laser Induced Breakdown Spectroscopy

> Number of measurements：输出次数（输出到Excel内的数据）
>
> Averages：平均次数（对所测量的数据平均多少次输出一次，在$$AutoSoft$$勾选的情况下）
>
> AutoSave\ Measurements(Save Spectra ......)：自动保存测量数据

![](https://gitee.com/lim-gitee/blog-image/raw/master/img/20201009101650.png)

​	5 点击OK保存，放置好样品即可开始测量
