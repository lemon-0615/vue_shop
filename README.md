# vue_shop
E-commerce management system
## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


## 过程笔记
###登录成功之后的操作：
<ol>
<li>把服务器给颁发的token信息记录到客户端的seisionStorage中，因为项目中除了登录之外的其他API接口，必须在登录之后才能访问，即给其他接口提供了身份验证信息</li>
```
 window.sessionStorage.setItem("token", res.data.token);
 ```
 <li>通过编程式导航跳转到后台主页，路由地址是/home<li>
  ```
  this.$router.push('/home')
  ```
  </ol>
