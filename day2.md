# Day2


#### 基本流程(React v18)
- import导入React、ReactDOM库
  - `import React from 'react';`
  - `import ReactDOM from 'react-dom/client';`
- 创建/引入App组件
  - `function App() {}`
  - `import App from './App'`
- 获取root元素
  - `const root = ReactDOM.createRoot(document.getElementbyId('root'));`
  - `root.render(<React.StrictMode><App /></React.StrictMode>)`
  - `root.render(<App />, document.getElementbyId('root'))`[v18 以前]

#### 三个核心概念
- **props**
  - 用于将数据从父组件传递到子组件(沿组件树向下)
  - 配置和定制组件的基本工具
  - 父组件控制子组件的外观和工作方式
- **components**
  - react应用程序完全由components构成
  - components是React中任何用户界面的构建块
  - 具有自己的数据、JavaScript逻辑和外观的UI片段
  - 通过构建多个组件构建复杂的UI
  - 组件可以重复利用，并且可以嵌套使用，进行数据传递
- **JSX**
  - 一种**声明性语法**，用于描述组件的外观及如何基于其数据和逻辑工作
  - components必须返回JSX块
  - JSX是JavaScript的拓展，允许将JavaScript、css和react组件嵌入进HTML中
  - 所有JSX元素都被`React.createElement()`调用进行转换
  - 可以使用没有JSX的React
 

#### &&/|| 和三元运算符
- && 渲染第一个为真的
- || 渲染第一个为假的
- 三元： `{num > 0 ? '' : ''}`




##### 样式
- 内联：
  - `<div style={{color : 'red', font-size:'32px'}}></div>`
- class
  - `<div className={`class1  ${_ ? '' : ''}`}></div>`
