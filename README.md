## 处理滚动穿透问题

### 外部滚动，内部也可以滚动（手机端和PC端均可以使用）

#### demo-all1.html

#### demo-all2.html

#### demo-all3.html（推荐）


### 外部滚动，内部不滚动

#### demo-mobile.html：手机端

方式一： 给modal容器添加 @touchmove.prevent

方式二：

```js
this.$refs.modal.addEventListener('touchmove', function (e) {
  e.preventDefault();
}, false);
```

#### demo-pc.html：PC端

方式一：给modal容器添加 @mousewheel.prevent

方式二：

```js
this.$refs.modal.addEventListener('mousewheel', function (e) {
  e.preventDefault();
}, false);
```
