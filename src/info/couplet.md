---
page: false
title: AD.js 对联广告
footer: false
---

# 横幅广告


## 示例
<script setup>
import Couplet from '@theme/examplate/couplet.vue'
</script>

<Couplet/>

## CDN
```html
  <div id="ad-couplet" style="background-color: red;float: right; width:100vw;height:10vw;"></div>

```

```js
  <script src="../../../dist/ad.js"></script>
  // 创建容器
  const couplet = document.getElementById('ad-couplet')
  // 初始化
  new AD.coupletAD(couplet, { appkey });
```

## NPM
```js
// @ts-ignore // ts忽略验证
import AD from 'adui.js'
const appkey = 'app1'

export default {
  data() {
    return {
      bannber: undefined,
    }
  },
  mounted() {
    const couplet = this.$refs['couplet']
    this.couplet = new AD.CoupletAD(couplet, { appkey });
  },
}
```

