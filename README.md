# CustomTabBarController

##多控制器管理
```
如果2个控制器的view是父子关系，那么这2个控制器也应该为父子关系
[vc01.view addSubview: vc02.view];
[vc01 addChildViewController: vc02];
// 会将vc02添加到vc01.childViewControllers数组中
```

##通过按钮点击来切换控制器view
```
需要保证控制器的添加顺序，这样在点击按钮时才能在childViewControllers数组中找到对应的控制器
```

##切换view的核心方法
```
-(void)switchToVC:(UIViewController *)newVC withAnimationType:(NSString *)type{}
```
