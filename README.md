# GridDividerItemDecoration
[简书相关介绍文章：https://www.jianshu.com/p/fb7e1a0749d6](https://www.jianshu.com/p/fb7e1a0749d6)

这个GridDividerItemDecoration适用于适用RecyclerView时，采用GridLayoutManager时，间隔计算问题：
具体为：
1. 可以在首尾列与父布局之间添加间隔
2. item可以自己设置宽高，也可以程序自己自动生成
3. 行与行之间的距离可以设置，列与列之间的距离自动计算

如图：

![行间距](https://github.com/haozi5460/GridDividerItemDecoration/blob/master/WX20181011-114206.png)

![列间距](https://github.com/haozi5460/GridDividerItemDecoration/blob/master/WX20181011-114222.png)

![与父控件间距](https://github.com/haozi5460/GridDividerItemDecoration/blob/master/WX20181011-114236.png)

解决的问题：
1. 解决搜索到的GridItemDecoration，不能添加首尾列与父布局之间间隔的问题
2. 解决item设置宽高后，列与列之间间隔大小不一的问题
3. 解决设置间隔后，item大小不一的问题等。。。

使用方法：
`
recyclerView.addItemDecoration(new GridDividerItemDecoration(this,Utils.dp2px(getContext(),20),Utils.dp2px(getContext(),15),true));`
                                

GridDividerItemDecoration构造函数有几种，分别可以设置是否需要添加首尾列与父布局之间间隔；是否需要添加第一行与父布局的间隔；最后一行是否需要间隔等
