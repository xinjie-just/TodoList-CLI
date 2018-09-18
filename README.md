# TodoList-CLI

## 项目安装
```
npm install
```

### 为开发进行编译和热重加载
```
npm run serve
```

### 编译和构建(用于生产环境)
```
npm run build
```

### 完善和格式化代码
```
npm run lint
```
1. main.ts(语言设置为 typescript 就是 main.ts)中引入 Vue,实例化 Vue 对象,和要显示视图的那个组件
2. public 存放了 ico 和 index.html，定义了根标签，作为 Vue 的挂载点
3. package.json 文件中配置了需要用到的插件的版本号，和启动命令
4. assets 中存放静态资源，如图片，图标，第三方插件等
5. components 文件夹中存放组件
6. 同直接引入 Vue 脚本比较，CLI 生成项目，更加符合工程化，更适合大型项目
7. 每一个组件，在一个文件中，方便维护
8. 每一个组件分为template，style，script 三部分
 * 模板写在 template 标签中，并且最外层只能有一个同级元素。
 * 样式写在 style 标签中，并可以通过设置 scoped 保证其作用于为当前组件，不影响父组件或子组件。
 * 逻辑写在 script 中，并可以通过 @import 导入其他组件