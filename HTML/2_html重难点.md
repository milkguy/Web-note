## 英语小课堂

`hyper` 超级    `target` 目标    `reference` 引用    `frame` 边框、框架   

 `error` 错误    `blank` 空白    `load` 加载    `canvas` 画布

##  a 标签

* href 超链接

  可链接的内容

  网址：

  1. https://google.com

  2. http://google.com

  3. [//google.com](//google.com)

  路径：

  	1. [/a/b/c](/a/b/c)
  	2. [index.html 或者./index.html]()

  伪协议：

  1. [javascript伪协议]()

     添加一个a标签，里面什么都不做<a href="javascript:;">javascript</a>

  2. id
  
4. [tel：手机号]()
5. Mailto

* target 在哪个窗口打开（_blank表示在空白页面打开）

  1. _blank 在新的页面打开
  2. _self 在当前页面打开
  3. _top 在顶级窗口打开超链接
  4. _parent 在父级窗口打开

* download 下载网页，一般没有用

* rel=nopener 修复bug

预览页面方法

	1. [http-server . -c-1]()
	2. [parcel 页面地址]()

程序员的命名

1. window的name
2. iframe的name

## iframe 标签

内嵌一个网站

## table 标签

<table>
  <thead>
    <tr>
    <th>表头</th>
    <th>表头</th>
    </tr>
  </thead>
  <tbody>
		<tr>
    <td>内容</td>
    <td>内容</td>
    </tr>
  </tbody>
  <tfoot></tfoot>
</table>

css样式：

​        table-layout: auto; 设置表内元素占用的距离，auto表示随着内容变化表格间距也发生变化

​		 **border-spacing: 0; 设置表格间距为0**

​        **border-collapse: collapse; 设置表格之间元素合并**

## img标签

* 作用：发出一个get请求，展示一张图片
* 属性
  1. alt 如果加载失败了，就显示alt
  2. height 高度
  3. width 宽度 （只写高度或者宽度，另一个能自适应）
  4.  src（source） 图片地址
  5.  onload js里监听图片加载成功
  6. onerror js里监听图片加载失败
  7. max-width：100%

## form 标签

* 作用：发get或post请求，然后刷新页面
* action：控制是哪个页面，一般来说是后端给路径 
* methon：get/post 控制是get还是post请求
* autocomplete：输入信息的时候给出自动建议
* target：选择在哪个页面提交
* onsubmit：测试提交

## input 标签

* 作用：让用户输入文本
* 属性type：
  1. button 按钮
  2. checkbox 多选，如果同一组的话，使用同一name属性
  3. email 邮箱📮
  4. file 上传文件，一般默认单个文件，上传多个文件的话属性后面添加multiple
  5. hidden 隐藏属性，一般用于js提交时使用
  6. number 输入数字
  7. password 输入密码
  8. radio 单选，如果设置多个选项为一组，只能选择同一个元素的话，使用同一name属性
  9. search 搜索栏
  10. submit 提交按钮，默认时提交，如果更改字的内容的话用value
  11. tel 手机号
  12. text 文本
  13. textarea 多行文本框，可以拖动，禁止拖动可以添加style属性，里面resize：none
  14. input submit和button区别：button里面还可以放其他东西，例如span，而且input submit里面不可以
  15. button里面必须有一个type="submit"才能提交表单
* onchange：用户输入改变的时候触发事件
* onfocus：用户鼠标聚焦时触发
* onblur：用户鼠标拿出来时触发
* HTML5：自带验证器（js中讲）
  1. required 必须填，否则不允许提交
* 一般不坚挺input里面的click事件
* form里面的input要有name
* form里面要放一个type=submit才能触发submit事件

## select 标签

* 作用：下拉标签
* option：填写标签内容
* value：依次填写

## textarea 标签

* 作用：输入多行文本
* style="resize: none"：表示不可调整大小，添加width和hight属性来控住输入框大小

* 注：
  1. 一般不监听input的click事件
  2. form里面的input都要有name （将http时提现）
  3. form里面要放一个sumbit才能出发submit事件