# AndroidUI For Web

移植Android的UI组件到Web端, 以Android的方式布局和处理界面.
[点击查看Sample](http://linfaxin.com/AndroidUI4Web/sample/main.html)


### 特点

1. 完整Native端组件体验
2. 高性能: 使用 Web Canvas 绘制UI, 还可以嵌入Runtime方法加速绘制
3. 可靠: UI组件由Android源码转换而来, 稳定可靠.
4. 拓展: 第三方Android UI库也可以移植到Web端.
5. 易用: HTML标签式声明组件.


### 60fps

达到60fps非常困难, 目前Sample页面在移动端的fps:

1. IOS:40fps左右
2. Android Chrome:30-40fps
3. Android WebView(4.4):20-30fps
4. Android Runtime:30-40fps


### 例子

```html
<android-Activity style="width: 100%; height:100%;display: none;">
    <ScrollView>
        <LinearLayout
                android:orientation="vertical"
                android:padding="12dp"
                android:gravity="center">
            <TextView >文本</TextView>
            <Button onclick="location.href='#'">按钮</Button>
        </LinearLayout>
    </ScrollView>
</android-Activity>
```
[点击查看Sample](http://linfaxin.com/AndroidUI4Web/sample/main.html)


### Runtime

使用Runtime加速后由原生端画布代替Web Canvas的绘制.

Android端Runtime Sample: [点击下载](http://faxin-10015149.file.myqcloud.com/AndroidUIRuntime.apk)
