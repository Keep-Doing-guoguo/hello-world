
# 1.Python
## 1.~取反操作
## 2.math.fmod(x, y) 方法返回 x/y 的余数。


# 2.Seaborn
## 1.sns.boxplot()#绘制箱型图，可以观察到异常值。  
## 2.sns.histplot()绘制直方图，需要bins。
## 3.heatmap绘制热力图。斯皮尔曼相关系数。
`sns.heatmap(numeric_feature.corr('spearman'),annot=True,fmt='g',cmap='Blues')`
## 4.countplot对数据中的某一特征进行计数，并且画图显示。
## 5.argsort()排序之后，返回的是索引。
## 6.sns.pairplot()用来展示两两特征之间的关系






# 3.Pandas
## 1.concat([a,b])拼接操作
## 2.groupby()分组操作
sum：是用来求和的  
agg：
`data.groupby('State').agg({'Yield':'max'})`取出来Yield这一个特征的最大值
## 3.
`pd.set_option('display.max_rows', 200)`  
`pd.set_option('expand_frame_repr', False)`
## 4.
## 3.merge()合并操作
## 4.quantile()表示分位数的意思，一般为0.25,0.5,0.75。分位数。
## 5.get_dummies()表示将使用哑变量。sklearn中的onehotencoder一样的效果。
## 6.检查缺失值
`data.info()`  
`data.isnull().sum()`

## 7.nunique()输出的是unique的数目
## 8.unique()输出的是单一的值
## 9.dropna()删除null值
## 10.nlargest()选择最大值，numpy也可以使用。
## 11.sort_values(ascending=False)ascending指的是上升的意思，为True就是。
## 12.drop_duplicates()删除重复的值
## 13.Dataframe中的value_counts()对种类进行分别计数。
`pd.to_datatime(df['arrival_year'].astype(str)+df['arrival_month'].astype(str),format='%Y%m')`
## 14.dropna(axis=0)将这一行其中有null的数据删除掉。对于少部分有null值的可以如何处理。
## 15.to_csv()将数据保存到本地文件。







# 4.Mataplotlib
## 1.一图多个的画法操作
这是第一种  
`plt.figrue()`  
`plt.plot()`  
`plt.show()`  
这是第二种  
`plt.figure()`  
`plt.subplot(1,3,1)`  
`sns.histplot()`  
`plt.subplot(1,3,2)`  
`sns.boxplot()`  
`plt.subplot(1,3,3)`  
`plt.plot()`  
这是第三种  
`fig,axs = plt.subplots(1,3)`  
`axs[0].`  
`axs[1].`





# 5.Numpy
## 1.np.where(condition,x,y)当where内有三个参数时，第一个参数表示条件，当条件成立时where方法返回x，当条件不成立时where返回y
## 2.np.bincount()将其从小到大进行排序，然后对每一个数值进行技术，并且返回技术结果的函数。
## 3.np.argmax()是找到array中最大值，并且返回最大值索引的函数。
## 4.np.floor()只保留小数的整数部分。
## 5.np.ceil()向上取整
## 6.np.full（）创建一个全部都是一个数字的矩阵。
## 7.np.clip（）设置一个上下界。
## 8.np.fliplr()将数组将数组从左向右翻转
## 9.np.ceil()取整函数
## 10.np.argsort()返回的是元素值从小到大排序后的索引值的数组



# 6.os
## 1.os.listdir()
## 2.os.path.join()
## 3.os.path.isdir()
## 4.os.path.exists()
## 5.os.rename()
## 6.os.getcwd()
## 7.os.makedirs()

# 7.opencv2

## 1.cv2.imraed()读取图片操作
## 2.cv2.blur()增加模糊程度
## 3.cv2.resize()改变图片大小
## 4.cv2.cvtColor()更换BGR或者RGB或者HSV的图片格式
## 5.cv2.merge()对通道进行合并

# 8.pytorch
## 1.expand_as()扩展张量，使得和原来张量大小相同。