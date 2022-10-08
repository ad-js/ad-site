---
page: false
title: AD.js 横幅广告
footer: false
---

# 横幅广告


## 示例
<script setup>
import rollup from '@theme/examplate/rollup.vue'
</script>

<rollup />

## CDN
```html
  <div id="ad-rollup1" style="background-color: red;float: right; width:100vw;height:10vw;"></div>

```

```js
  <script src="../../../dist/ad.js"></script>
  // 创建容器
  const rollup1 = document.getElementById('ad-rollup1')
  // 初始化
  new AD.rollupAD(rollup1, { appkey });
```

## NPM
```js
// @ts-ignore // ts忽略验证
import AD from 'adui.js'
const appkey = 'app1'

export default {
  data() {
    return {
      rollup: undefined,
    }
  },
  mounted() {
    const rollup = this.$refs['rollup']
    this.rollup = new AD.rollupAD(rollup, { appkey });
  },
}
```

