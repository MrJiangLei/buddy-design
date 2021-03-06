## Navbar 导航栏

顶部导航栏，支持深色背景和白色背景，如果要自定义背景色，请根据 `自定义主题` 章节进行自定义

### 按需引入

```javascript
import Vue from 'vue'
import { Navbar } from 'buddy-design'

Vue.use(Navbar)
```

### 基本用法

```html
<wd-navbar title="标题"></wd-navbar>
```

设置 `left` slot。

```html
<wd-navbar title="左侧文字">
  <div slot="left">
    <wd-icon class="middle" name="arrow-left" />
    <span class="middle">返回</span>
  </div>
</wd-navbar>
```

设置 `right` slot。

```html
<wd-navbar title="右侧文字">
  <span slot="right">菜单</span>
</wd-navbar>
```

同时设置。

```html
<wd-navbar title="左右侧文字">
  <div slot="left">
    <wd-icon class="middle" name="arrow-left" />
    <span class="middle">返回</span>
  </div>
  <span slot="right">菜单</span>
</wd-navbar>
```

如果标题文案过长，则会省略号显示。

```html
<wd-navbar title="标题的字数如果太多则超出隐藏">
  <div slot="left">
    <wd-icon class="middle" name="arrow-left" />
    <span class="middle">返回</span>
  </div>
</wd-navbar>
```

### light 主题

设置浅色主题。

```html
<wd-navbar title="标题" light></wd-navbar>
```

### Attributes
| 参数      | 说明                                 | 类型      | 可选值       | 默认值   |
|---------- |------------------------------------ |---------- |------------- |-------- |
|title      |	标题                                |	string    |	—           |	—       |
|light	    | 是否使用白色背景                      |	boolean    |	-         |	false |

### Slot
| name      | 说明       |
|------------- |----------- |
|left         | 左侧操作 |
|right        | 右侧操作 |
