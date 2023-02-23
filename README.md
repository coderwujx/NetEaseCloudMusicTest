# React 实战之云音乐项目

### 1.项目规范

**项目规范：项目中有一些开发规范和代码风格**

- 1.文件夹、文件名称统一小写、多个单词以连接符（-）连接；
- 2.JavaScript 变量名称采用小驼峰标识，常量全部使用大写字母，组件采用大驼峰；
- 3.CSS 采用普通 CSS 和 styled-component 结合来编写（全局采用普通 CSS、局部采用 styled-component）;
- 4.整个项目不再使用 class 组件，统一使用函数式组件，并且全面使用 Hooks；
- 5.所有的函数式组件，为了避免不必要的渲染，全部使用 memo 进行包裹；
- 6.组件内部的状态，使用 useState、useReducer；业务数据全部放在 redux 中管理；
- 7.函数组件内部基本按照如下顺序编写代码：
  - 组件内部 state 管理；
  - redux 的 hooks 代码；
  - 其他组件 hooks 代码；
  - 其他逻辑代码；
  - 返回 JSX 代码；
- 8.redux 代码规范如下：
  - redux 结合 ImmutableJS
  - 每个模块有自己独立的 reducer，通过 combineReducer 进行合并；
  - 异步请求代码使用 redux-thunk，并且写在 actionCreators 中；
  - redux 直接采用 redux hooks 方式编写，不再使用 connect；
- 9.网络请求采用 axios
  - 对 axios 进行二次封装；
  - 所有的模块请求会放到一个请求文件中单独管理；
- 10.项目使用 AntDesign
  - 项目中某些 AntDesign 中的组件会被拿过来使用；
  - 但是多部分组件还是自己进行编写；
- 其他规范在项目中根据实际情况决定和编写；

### 2. 项目运行

clone 项目：

```
git clone https://github.com/coderwujx/NetEaseCloudMusicTest.git
```

安装项目依赖：

```shell
yarn install
```

项目运行：

```shell
yarn start
```
