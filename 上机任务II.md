首先，请选择性练习下面各章的 plot 方法。

接着，基于ggplot2,用violin plot对iris数据集中不同Species的Sepal.Length长度分布进行可视化，并进行如下设置。画violin plot时可参考 2a)，对作图进行配置还可以参考本节的 1d) 和7)。 提交脚本和结果。

把图片标题设为"Sepal Length Distribution"，加粗居中(可使用labs函数和theme函数)

把y轴范围设为0.5到7之间(可使用scale_y_continuous函数)

三个Species的对应的填充颜色分别设为#C44E52, #55A868和#4C72B0(可使用scale_fill_manual函数)

---

**code:**
```R
library(ggpolt2) #导入ggpolt2包
ggplot(iris,aes(x=Species,y=Sepal.Length,fill=Species)) #创建图表
+ labs(title="Sepal Length Distribution",x="Species",y="Sepal.Length") #设置图表标题内容
+ geom_violin() #绘制violin图
+ theme(plot.title = element_text(hjust = 0.5,face = "bold")) #设置标题格式加粗居中
+ scale_fill_manual(,"Species",values = c("#C44E52", "#55A868","#4C72B0")) #设置图表填充颜色
+ scale_y_continuous(breaks=seq(0.5,7,by = 0.5),limits = c(0.5,7))  #设置y轴范围
```

**result：**
![image](https://github.com/GodLemma/Bioinformatics/assets/162097106/adafb664-b116-4728-ab5b-b4718329d8d3)

