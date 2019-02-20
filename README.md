# SHTimer
# 如何使用：
## 1. 调用
### 创建一个NSString字符串，用来接收返回值（timer的唯一标识）
    self.task = [SHTimer execTask:self
                         selector:@selector(doTask)
                            start:2.0
                         interval:1.0
                          repeats:YES
                            async:NO];
## 2. 取消
### 直接在要取消的地方调用cancle方法
- (void)touchesBegan:(NSSet<UITouch *> *)touches withEvent:(UIEvent *)event
{
    [SHTimer cancelTask:self.task];
}
