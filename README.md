# echarts3_map_demo
效果预览：http://htmlpreview.github.io/?https://github.com/lixinGiting/echarts3_map_demo/blob/master/index.html

内容说明：利用ECharts3来实现ECharts2实例中的模拟迁徙效果，即背景地图为百度地图。

背景介绍：
    与echarts2相比echarts3有很大的改动。
    ECharts2推荐模块化单文件引入；由于echarts依赖底层zrender，你需要同时下载zrender到本地。ECharts3开始不再强制使用 AMD 的方式按需引入，代码里       也不再内置 AMD 加载器。因此引入方式简单了很多，只需要像普通的 JavaScript 库一样用script标签引入。 
    ECharts3中因为地图精度的提高，不再内置地图数据增大代码体积，你可以在地图下载界面下载到需要的地图文件引入并注册到 ECharts 中。
    
    如果采用echarts3官方给的地图加载方式那么会得到和echarts3官方实例一样的黑色背景的地图。
    echarts2中的模拟迁徙之所以能显示百度地图的背景，是因为它引入了百度地图，百度地图和echarts2的结合比较简单，官方也有很多百度地图的扩展实例。
    重点是echart3和百度地图的结合，需要引入百度开发者密钥，还要引入bmap文件，否则会报错。百度开发者密钥去百度地图API官网申请即可，很简单。

文件介绍：bmap.js 背景地图所需的依赖文件
        echarts.js  使用ECharts3所必须的文件
        index.html 展示界面
        text.js   可以自由定制的js文件
