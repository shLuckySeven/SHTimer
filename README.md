# SHTimer
A comfortable using the timer
# 如何使用：
## 1. 调用
### 接口设计
    self.task = [SHTimer execTask:self
                         selector:@selector(doTask)
                            start:2.0
                         interval:1.0
                          repeats:YES
                            async:NO];
