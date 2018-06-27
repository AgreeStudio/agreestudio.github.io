#  使用手册
## 1. 工程相关操作

### 1.1 创建工程
1. 顶部菜单栏选择 [工程] - [创建工程]
2. 选择工程类型,填写工程项目信息,[应用名称],[应用说明],[应用地址]----工程文件要保存的地址,默认为workspace路径下。
![创建工程](/images/user-guide/创建工程.gif)
3. 点击[完成]后,工程创建成功,在左侧导航栏区域即可查看到当前创建的工程

### 1.2 切换工程
1. 顶部菜单栏选择 [文件] - [切换工程] 显示了当前工作空间可供切换的全部工程，点击某个工程即可切换
![切换工程](/images/user-guide/切换工程.png)

### 1.3 启动工程

1.  顶部菜单栏选择 [文件] - [启动工程] 用以启动工程，只有当工程正常启动后，vueEditor 才可以正常工作。
2.  当用户创建，导入，切换工程时，AgreeStudio 会默认启动工程，但当工程由于某些原因无法启动时，需要用户先处理问题再手动启动工程。
3.  启动工程时，AgreeStudio 能简单提示工程是否启动，以及失败原因以及错误码。
    ![切换工程](/images/user-guide/启动工程.jpg)


## 2. 工程文件(夹)相关操作

### 2.1 新建文件(夹)
1. 在文件树文件(夹)右键 - [新建文件(夹)]
![新建文件](/images/user-guide/新建文件1.png)
2. 在对话框中输入文件(夹)名
![新建文件](/images/user-guide/新建文件2.png)
3. 文件名通过校验后，创建文件(夹)成功
![新建文件](/images/user-guide/新建文件3.png)

### 2.2 打开文件
- 文件树点击文件即可打开文件
- 对于 `.vue` 和 `.json` 文件，默认使用可视化编辑模式打开，可通过文件树选择文件并右键 - [打开方式] 选择文本打开方式
![打开文件](/images/user-guide/打开文件.gif)

### 2.3 重命名文件(夹)
1. 在文件树文件(夹)右键 - [重命名]
![重命名文件](/images/user-guide/重命名文件1.png)
2. 在对话框中输入新文件名
![重命名文件](/images/user-guide/重命名文件2.png)
3. 文件名通过校验后，重命名文件成功

### 2.4 删除文件(夹)
1. 在文件树文件(夹)右键 - [删除]
![删除文件](/images/user-guide/删除文件.png)

### 2.5 在资源管理器中显示
1. 在文件树文件(夹)右键 - [在资源管理器中显示]
![在资源管理器中显示](/images/user-guide/在资源管理器中显示.png)

### 2.6 查看文件(夹)属性
1. 在文件树文件(夹)右键 - [属性]
![查看属性](/images/user-guide/查看属性.gif)

## 3. 项目开发

### 3.1 vue文件编辑
  *在文件树单击或右键选择vue_editor即可以可视化编辑方式打开vue文件*
  #### 页面编辑
  *左侧选择 [页面] 进入页面编辑模式*
  - 添加组件
    在左侧工具栏中选择某个组件、拖动至页面中即可快速的在页面中添加一个组件
    ![添加组件](/images/user-guide/添加组件.gif)
  - 修改组件属性
    选中某个组件，右侧属性区显示了该组件的所有属性，选择某一属性即可编辑，并支持添加自定义属性、绑定动态属性值
    ![修改组件属性](/images/user-guide/修改组件属性1.gif)
    ![修改组件属性](/images/user-guide/修改组件属性2.gif)
  - 删除组件
    选中某个组件，顶部右侧工具栏中删除按钮即变为激活状态，点击删除按钮即可删除该组件
    ![删除组件](/images/user-guide/删除组件.gif)
  - 组件事件绑定
    选中组件，在右侧事件区显示了可供绑定的事件，下拉菜单中显示了methods域的方法，选择某一方法即可为组件绑定事件，并支持绑定自定义事件
    ![组件绑定事件](/images/user-guide/组件绑定事件.gif)
  - 页面整体编辑
    可通过拖拽、点击等方式进行复杂的编辑，左侧导航区选择 [大纲] 可显示当前页面的组件结构并进行联动操作
    ![页面整体编辑](/images/user-guide/页面整体编辑.gif)
  - 项目预览
    在可视化编辑视图顶部工具栏可以预览项目的运行状态、横竖屏显示、缩放比例、更改设备等操作
    ![项目预览](/images/user-guide/项目预览.gif)
  #### 逻辑编辑
  *左侧选择 [逻辑] 进入逻辑编辑模式*
  - data域
    data域可编辑文件的data数据部分，复杂数据类型可使用json可视化编辑方式 [参考 3.2 json文件编辑]
    ![data域](/images/user-guide/data域.gif)
  - methods域
    methods域可编辑文件的methods数据部分
    ![methods域](/images/user-guide/methods域1.gif)
    在methods域点击右上角按钮可以快速引入`Aui`、`AgreeSDK`代码
    ![methods域](/images/user-guide/methods域2.gif)
  - computed域
    computed域可编辑文件的computed数据部分
    ![computed域](/images/user-guide/computed域.gif)
  - watch域
    watch域可编辑文件的watch数据部分
    ![watch域](/images/user-guide/watch域.gif)
  - 生命周期域
    生命周期域可以绑定生命周期函数
    ![生命周期域](/images/user-guide/生命周期域.gif)
  - 总览
    总览区以文本方式展示了vue文件的`script`标签部分的全部内容
    ![总览](/images/user-guide/总览.png)
  #### 样式表编辑
  *左侧选择 [样式表] 进入样式表编辑模式*
  - 样式表编辑<p>
    这里可以修改Vue文件的style节点的样式表<p>
    样式表目前默认为全局样式表，scope域在未来版本加入
    ![样式表编辑](/images/user-guide/stylesheet.gif)
  - 组件的样式编辑(element.style)<p>
    在页面选项卡选中组件，在右侧页面点击样式选项卡，单击element.style区域，就可以编辑组件样式。编辑完成后需要点击保存按钮。
    ![组件的样式编辑](/images/user-guide/elementstyle.gif)
  - 查看当前选中组件的样式表<p>
    点击组件，在右侧展示当前组件的所有样式表
  
    ![查看当前选中组件的样式表](/images/user-guide/findstyle.gif)
  - 查看当前命中样式表会影响哪些组件<p>
    将鼠标悬浮到样式表上，就可以在页面区域看到影响的组件背景变蓝了
  
    ![查看当前命中样式表会影响哪些组件](/images/user-guide/findelement.gif)
  - 样式表的添加<p>
    将鼠标悬浮到任意样式表上，点击左上角的添加按钮
  
    ![样式表的添加](/images/user-guide/styleadd.gif)
  - 样式表的删除<p>
    将鼠标悬浮到要删除的样式表上，点击左上角的删除按钮
    ![样式表的删除](/images/user-guide/styledelete.gif)
  - 样式表的修改<p>
  
    ![样式表的修改](/images/user-guide/stylemodify.gif)
    点击要修改的样式表，就可以编辑该样式表


### 3.2 自定义组件
  1.在`{当前开发工程}/src/custom-components`文件夹右键 - [新建自定义组件] 输入自定义组件名称即可快速创建一个自定义组件
  ![创建自定义组件](/images/user-guide/创建自定义组件.gif)
  2.选择`{自定义组件名称}.vue`文件以添加页面元素与属性、事件等内容
  ![编辑自定义组件内容](/images/user-guide/编辑自定义组件内容.gif)
  3.选择`{自定义组件名称}.definition.json`文件，编辑该自定义组件的名称、描述、属性、事件等信息
  ![编辑自定义组件定义](/images/user-guide/编辑自定义组件定义.gif)
  4.点击下方[保存并同步到AgreeStudio]按钮，即可在工具箱中显示
  5.在工程页面中使用该组件
  ![使用自定义组件](/images/user-guide/使用自定义组件.gif)

### 3.3 json文件编辑
  json类型文件支持可视化编辑方式
  ![jsonEditor](/images/user-guide/jsonEditor.gif)

### 3.4 其他类型文件编辑
  其它文本类型文件使用文本编辑器编辑
   ![文本编辑器](/images/user-guide/文本编辑器.gif)

### 3.5 图片预览
  图片类型支持图片预览、缩放操作
  ![图片预览](/images/user-guide/图片预览.gif)

### 3.6 控制台
  通过控制台可以进行命令行相关操作
  ![控制台](/images/user-guide/控制台.png)

### 3.7 快捷操作
  Agree Studio支持如下快捷操作：
  - 快速关闭标签页
    1. 关闭当前标签页 `Alt + c`
    2. 关闭全部标签页 `Alt + a`
    3. 关闭左侧标签页 `Alt + p`
    4. 关闭右侧标签页 `Alt + n`
    5. 关闭其它标签页 `Alt + s`
  ![快捷操作](/images/user-guide/快捷操作1.gif)

## 4. 项目调试
  支持通过devTools面板进行调试，可通过如下方式打开调试面板：
  1. F12热键打开
  2. 顶部菜单栏选择 [帮助] - [打开开发者工具]

## 5. 构建工程
  1. 顶部菜单栏选择 [文件] - [构建工程]
  2. 等待底部状态栏显示 `工程构建成功` 即为构建成功，相关文件保存在`{Agree Studio安装目录}\studiobuild\app\build`下
  ![构建工程](/images/user-guide/构建工程.png)

## 6. 错误码说明：

| 错误码 |          描述           |
| :----: | :---------------------: |
|  400   |      invalid param      |
|  401   |      unauthorized       |
|  403   |        forbidden        |
|  404   |        not found        |
|  500   |  internal server error  |
|  503   |      service busy       |
|  1301  |     file not exists     |
|  1401  |    no active project    |
|  1402  | node_modules not exists |
|  1403  | project already started |