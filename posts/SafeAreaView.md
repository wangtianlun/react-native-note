# SafeAreaView

SafeAreaView的作用是在一个设备的安全界限之内来渲染内容，一般应用在IOS上，并且要求版本在IOS11以上

用SafeAreaView来渲染内容，它会自动适配内边距的部分，所以它不会被导航条，tab条，工具条，或者其它祖先View覆盖，此外，最重要的, 安全区域内边距反应了屏幕的物理限制，比如圆角和相机槽（例如：在iphoneX上的传感器坐落的区域）

### 使用方式

  在你的顶层容器外包裹一层SafeAreaView，可以应用一个“flex: 1”的样式

  ```javascript
    <SafeAreaView style={{flex: 1, backgroundColor: '#fff'}}>
      <View style={{flex: 1}}>
        <Text>Hello World!</Text>
      </View>
    </SafeAreaView>
  ```