# Camera-of-LiaoNing-Robocon-2017
Golf ball recognition in LiaoNing robot contest 2017

please use multiSend branch


### 存在问题

1. 场地边缘的半个球识别不到
2. 创建滑动条方便进行调参
3. 补光灯选型
4. cmake管理工程
5. 如果看到了场地外的绿色区域，则寻找最大凸包去除场地外绿色干扰
6. 场地边缘有时会被识别为球，需要进一步处理
7. 敌方车干扰问题
8. 中央高空储藏室架子问题以及网兜内球的问题
9. 黑球空缺填补
10. 环境自动调整（未解决，正在买灯）
  * 自动白平衡已实现
  * 自动亮度存在超调现象
  * 由于太暗导致色差太小，尝试自动对比度
11. 开机时间过长报错VIDIOC_DQBUF no such device
12. 过大或过小连通域的去除
    * `NoBGBallImage`内去除过大与过小连通域
    * 在`getImage()`内进行操作
13. 橙色 蓝色 红色背景加入球的识别范围


* 霍夫变换不能解决环境光照改变的本质问题

