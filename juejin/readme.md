## css 预编译语言 stylus
写的是stylus .styl 在浏览器段运行的是.css
前端工作流在发生改变
界面开发工作被重新定义了，从小米加步枪变生产线
stylus main.styl -o main.css
编译功能 -o 输出，将styl 文件输出为 css文件
stylus 提供了css不具备的变量定义，模块化 ，函数，快捷，新的语法
-w watch 监听文件修改，同时编译
在兄弟之间 一个图片和一段文字 ，要垂直居中对齐，1.设置img 属性 ：vertical-align：middle
                                            2.添加弹性布局，display：inline-flex
                                              align-items ：center

1.变量
2.减少输入 {} ; :
3.函数
4.嵌套
.book-bought 购买模块
  .lable
    img
& 引用上一级的层次类名，同时可以缩进
省去重复上一次的选择
.user:fisrt-child = &:fisrt-child
flex 是css  在移动时代最爽的布局方案，手机端子元素们对齐方式，
水平 主轴 justify-content
纵轴 align-items ：center
传统方案是img+兄弟结点 设置  vertical-align：middle

flex 考点  自适应
1.flex：1 比例划分，只给一个元素设置，他将占据其他元素外的所有
2.父元素与多个子元素之间的关系
水平对齐  justify-content
垂直对齐 align-items
3.剩余空间 flex-grow ：1 为1时就是把剩余空间都给该元素
4. flex-wrap: wrap;  /*一行放不下就放下一行*/
5. flex-shrink: 1;
超出的时候按比例缩小
