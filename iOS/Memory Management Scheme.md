# 内存布局


![风景图](https://baidu.com)

## 内存管理方案
 - 实例方法调用时，通过对象的 isa 在类中获取方法的实现
 - 类方法调用时，通过类的 isa 在元类中获取方法的实现

## 数据结构


## 引用计数原理

 ### ARC auto refrence counting
描述：
 ### MRC
- alloc
- retain
- retainCount
- release/autorelease



引用计算产生什么题？
循环引用/内存泄漏/野指针/ --> 卡死/崩溃

怎么解决这些问题
自动释放池
weak弱引用实现原理
weak实现原理

```objectivec
XXObject *xx = [[XXObject alloc] init]
YYObject *yy = [[YYObject alloc] init]
objc_msgSend(xx, @selector(hello))
objc_msgSend(yy, @selector(hello))
```

![结构脉络](./images/Block.png)
