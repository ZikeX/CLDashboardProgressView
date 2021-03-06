# CLDashboardProgressView 1.0
仪表盘样式的进度条

<br />
作者：李辉 <br />
联系方式：6545823@qq.com <br />
编译环境：Xcode 7.2 <br />
运行环境：iOS 9.2 运行正常 <br />
您在使用该控件的过程中，如有任何疑问或建议，请通过邮箱联系我，谢谢！ <br />

<br />
![image](https://github.com/changelee82/CLDashboardProgressView/raw/master/Demo.gif)
<br />

使用方法
===============
可使用自动布局或代码添加该控件； <br />
    _progress = [[CLDashboardProgressView alloc] initWithFrame:CGRectMake(20, 60, 240, 240)];
    _progress.center = CGPointMake([UIScreen mainScreen].bounds.size.width * 0.5, 190);
    _progress.backgroundColor = [UIColor blackColor];
    
    _progress.outerRadius = 110; // 外圈半径
    _progress.innerRadius = 95;  // 内圈半径
    _progress.beginAngle = 90;   // 起始角度
    _progress.blockAngle = 8;    // 每个进度块的角度
    _progress.gapAngle = 2;      // 两个进度块的间隙的角度
    _progress.progressColor = [UIColor greenColor]; // 进度条填充色
    _progress.trackColor    = [UIColor redColor];   // 进度条痕迹填充色
    _progress.outlineColor  = [UIColor grayColor];  // 进度条边框颜色
    _progress.outlineWidth  = 2;                    // 进度条边框线宽
    
    _progress.blockCount = 26;   // 进度块的数量
    _progress.minValue = 0;      // 进度条最小数值
    _progress.maxValue = 100;    // 进度条最大数值
    _progress.currentValue = 10; // 进度条当前数值
    
    _progress.showShadow = YES;       // 是否显示阴影
    _progress.shadowOuterRadius = 85; // 阴影外圈半径
    _progress.shadowInnerRadius = 10; // 阴影内圈半径
    _progress.shadowFillColor = [[UIColor grayColor] colorWithAlphaComponent:0.3];   // 阴影颜色
    
    _progress.autoAdjustAngle = YES;  // 自动调整角度，使开口向下
    
    [self.view addSubview:_progress];
    
详细的示例请参考代码。 <br />

历史版本
===============
v1.0 - 2015-12-18 <br />
Added <br />
基础功能完成 <br />
