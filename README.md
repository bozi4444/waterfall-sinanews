# waterfall-sinanews
## 瀑布流新闻网站
预览地址：
## 懒加载原理
开始所有图片的src都是同一个地址，实际上只有一个网络请求，其他的走缓存。真实地址放在自定义的属性中，
把刚开始就出现在窗口中，和滚动鼠标后出现在窗口中图片的src地址，变成真正的地址，显示图片。
## 瀑布流原理
初始化一个数组存储每一列高度都为0，排列图片时，选择高度最短的那列，把图片放在那列下面，
比如第一次排列图片，把他放在第一列下面，那么第一列的高度变为此图片的高度。然后继续按照这个规则排列
图片。
## 实现原理
1,实现page=1 的10条数据
2，把10条数据拼装成dom 放到页面
3，使用瀑布流去摆放dom 的位置
4，page++
当lead出现在眼前时
1,实现page 的10条数据
2，把10条数据拼装成dom 放到页面
3，使用瀑布流去摆放dom 的位置
4，page++