0行代码设置UINavigationBar无Back文字   

一般的，UINavigationController push完界面后，左上角会出现一个小左箭头，同时会出现“Back”（如果真机是中文则是显示“返回”）。
但是怎么消除文字只要左箭头呢，一般的情况是自定义UIBarButtonItem，然后设置setLeftBarButtonItem。
这样的导致的问题有很多，如果你的工程中调用类似UIImagePickerController这样的原生类是无济于事的。而且如果本身使用的是iOS 7原生的侧滑返回（如果你不用第三方的侧滑返回），这样的效果是会失效的。
想了下，写了个demo出来。解决了如下问题，1.消除返回的“Back”文字。2.自定义小箭头的frame。
代码直接拖到工程中即可使用。简单方便。希望你喜欢。。。
