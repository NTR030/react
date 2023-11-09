# Day 3


#### useState
- import导入
  - `import { useState } from "react";`
- 创建状态
  - `const [data,setData] = useState()`
- 更改状态
  - `setData(n => n + 1)`


#### state指导方针
- 为组件随时间跟踪的任何数据创建一个新的状态变量(在未来某个时刻需要改变的变量)
- 希望组件中的某些内容是动态时，为其创建状态变量
- 改变组件的外观/显示的数据，通过set函数更新状态即可
- 不要为组件中每个变量创建状态


#### children
- 对于需要重复利用，且中间内容变化的组件，可以通过内置的prop.children是实现
  - 例如 `function Btn({children}){
  return (
    <button className='btn'>{children}</button>
}`
    - <Btn>-<Btn> 即可让中间的值为“-”
   

#### map指定长度循环渲染
`
{Array.from({length : 5},(_,i) => <option value={i + 1} key={i}>{i+1}</option>)}
`

#### 更新数组类型的state
- state初始值为[]，`setArr(arr =>arr.concat(new) )`
- state存在值，新增/改替数据 `setArr(arr => arr.toSpliced(index,1,new))`
- 清空state中的值 `setArr(arr => arr.toSpliced(0,arr.length))`
