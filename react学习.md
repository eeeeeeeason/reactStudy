# react学习

- helloWorld应用依赖于balbelstandalone可以把react的虚拟dom渲染进行render函数调用，但是受到实时es6转es5影响，效率极低

- 箭头函数不能直接使用，要在babelrc中添加预设stage-0

- 子类接收传递参数

  - ```js
    constructor(props){
      super()
      this.state = {count:props.initCount} // 赋值给子组件
    }
    static defaultProps = {
      initCount : 3000 //设置默认值
    }
    static propTypes = {
      initCount : PropTypes.number
    }
    //static defaultProps设置父组件传递的默认值 ，prop-types限制传递数据类型
    ```

  - ​

- 使用Create-React-App来建立TypeScript的环境

  ```
  npm i -g create-react-app
  create-react-app tinylog-ui --scripts-version=react-scripts-ts
  cd tinylog-ui/
  npm start
  npm run eject
  ```

  ​