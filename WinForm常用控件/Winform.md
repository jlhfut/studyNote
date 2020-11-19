#### Button 控件属性： 常用事件 click mouseEnter

​	**name:**

在后台要获得前台的控制对象，需要使用Name属性

**Visible：**

是否可见

**enable：**

指示控件是否可用

**text:**

设置控件名



#### 事件：发生的一件事件 ####

注册事件：双击闪电图标 Click

触发事件：点击

```c#
private void button1_Click(object sender,EventArgs e)

{

    Button btn=(Button)sender;
    MessageBox.Show("转换成功");
​	 //MessageBox.Show("Hello Word");

}
```



### 每个窗体都相当于一个类

 既然是一个类就需要使用new关键字来创建他，创建完对象后需要调用show()方法来显示窗体

```c#

Form2 frm2=new Form2();

//展示当前窗体

frm2.Show();

```



### Text 控件

  **属性 **：

​		ScrollBars: 滚动条 可以设置横向或者纵向；

​		WordWrap：指示文本框是否换行；

​		PasswordChar：让文本框显示一个单一的字符；



#### 事件

TextChanged   控件上更改Text属性的值引发的事件



### Timer 组件

**属性 ：**

​	Tick：每当经过指定的时间间隔时发生



记事本



### 单选 radioButton

### 多选 CheckBox



**属性 **

checked：指示这个控件是否处于选中状态（boolean)

默认情况下，在一个窗体中，所有的单选按钮只允许选中一个，可以使用groupbox进行分组

给控件分组：

为什么要分组：想要选择多个

***要用到容器：groupBox***



### MDI窗体设计

1.首先确定父窗体  将IsMdiContainer 设置为true

2.创建子窗体，并且设置父窗体



### picBox 窗体

上一张，下一张





