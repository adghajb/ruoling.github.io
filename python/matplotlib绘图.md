[Bar Chart Race in Python with Matplotlib](https://towardsdatascience.com/bar-chart-race-in-python-with-matplotlib-8e687a5c8a41)


散点图1

```py

import matplotlib.pyplot as plt
import matplotlib

#plt.plot(x,y,fomat_string,**kwargs)
#x:x轴数据，列表或数组
#y:y轴数据，列表或数组
#fomat_string:控制曲线的格式,fomat_string由颜色，风格，标记组成
#:多组(x,y,fomat_string)


#matplotlib.rcParams['font.family']='simHei'#将字体改为汉字中的黑体
plt.subplot(2,1,1)#绘图区域分成2行1列，并选择第1个区域
plt.plot([3,1,4,5,2])#会被当做y轴，x轴为索引
#plt.ylabel("纵轴(值)",fontproperties="simHei",fontproperties=20)#y轴名字用汉字中的黑体显示,字号为20
#plt.xlabel('横轴(值)',fontproperties="simHei",fontproperties=20)#x轴名字用汉字中的黑体显示,字号为20
plt.title()#加上标题
plt.text()#加上文本

#plt.savefig('文件名' , dpi=600)#保存为文件  #PNG文件
plt.show()

plt.subplot(2,1,2)
plt.plot([0,2,4,6,8],[3,1,4,5,2],'b*')
plt.ylabel("Grade")
plt.axis([-1,10,0,6])#y轴起始，x轴起始
plt.show()

```

散点图2

```py

import numpy as np
import matplotlib.pyplot as plt

fig, ax = plt.subplots()
ax.plot(10*np.random.randn(100), 10*np.random.randn(100), 'o')
ax.set_title('Simple Scatter')#标题

plt.show()

```



直方图

```py

import numpy as np
import matplotlib.pyplot as plt

np.random.seed(0)
mu, sigma = 100, 20   #均值和标准差
a = np.random.normal(mu, sigma, size=100)

plt.hist(a, 20, histtype='stepfilled', facecolor='r', alpha=0.75)
#20为个数
plt.title('Histogram')#名称
plt.ylabel('Y')#Y轴名称
plt.xlabel('X')#X轴名称

plt.show()

```

饼图

```py

#plt.pie
import matplotlib.pyplot as plt

labels = 'Frogs', 'Hogs', 'Dogs', 'Logs'#标签
sizes = [15, 30, 45, 10]
explode = (0, 0.1, 0, 0)#比例,0.1的将会突出

plt.pie(sizes, explode=explode, labels=labels, autopct='%1.1f%%',shadow=False, startangle=90)
plt.title('pie')#名称

plt.axis('equal')
plt.show()

```


极坐标

```py


#极坐标
import numpy as np
import matplotlib.pyplot as plt

N = 20#数据个数
theta = np.linspace(0.0, 2 * np.pi, N, endpoint=False)
radii = 10 *np.random.rand(N)
width = np.pi / 4 * np.random.rand(N)

ax = plt.subplot(111, projection='polar')
bars = ax.bar(theta, radii, width=width, bottom=0.0)

for r, bar in zip(radii, bars):
    bar.set_facecolor(plt.cm.viridis(r / 10.))
    bar.set_alpha(0.5)

plt.show()

```

