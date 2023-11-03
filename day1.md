# day1


#### 为什么需要框架
- 保持用户界面和数据同步（data <=> UI）
- 强制执行一种正确的结构和编写代码的方式（固定格式、代码风格）


#### react VS vanilla-js
- react中js负责一切；vanilla-js中HTML占据主导地位
- react不需要选择DOM元素；vanilla-js需要手动选择DOM元素
- react更新数据时会自动更新用户界面；vanilla-js需要手动进行页面更新


#### 什么是react
- 由Facebook创建的一个流行的，基于组件的，状态驱动的，用于构建用户界面的JavaScript库
  - 基于组件
    - 组件是react中用户界面的构建块
    - react基本上是获取组件并将其绘制在网页上
    - 重复利用组件
  - 声明性
    - 使用JSX的声明性语法描述组件的外观和工作方式
    - 根据当前数据/状态告诉react组件应该是什么样子
    - 不接触DOM，远离DOM的抽象
  - 状态驱动
    - react通过重新渲染UI对状态变化做出反应
  - JavaScript库
    - react本身只是**视图层** （缺少图路由等其它功能）
  - 流行性
    - 很多大公司正在使用react
    - 众多工作岗位
    - 活跃且庞大的社区
  - facebook创建
    - Jordan Walke 2011年创建
    - 2013年开源
   

#### react构建工具
- creact-react-app
  - 一个完整的react应用程序初学者工具包
  - 已**预先配置**所有常见的开发者工具(ESLint,Prettier...)
  - 使用了过时的技术(特别是webpack插件)
  -  **不建议使用creat-react-app用于真实项目**
- Vite
  - 一个现代构建工具，包含用于设置全新React应用程序的启动模板
  - 需要**手动设置**开发者工具(ESLint,Prettier...)
  - **热模块切换**，能够非常快的自动刷新页面
  - **Vite是构建真实项目的最好选择**
  

    
