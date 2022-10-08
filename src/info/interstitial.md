---
page: false
title: AD.js 横幅广告
footer: false
---

# 横幅广告


## 示例
<script setup>
import interstitial from '@theme/examplate/interstitial.vue'
</script>

<interstitial />

## CDN
```html
  <div id="ad-interstitial1" style="background-color: red;float: right; width:100vw;height:10vw;"></div>

```

```js
  <script src="../../../dist/ad.js"></script>
  // 创建容器
  const interstitial1 = document.getElementById('ad-interstitial1')
  // 初始化
  new AD.interstitialAD(interstitial1, { appkey });
```

## NPM
```js
// @ts-ignore // ts忽略验证
import AD from 'adui.js'
const appkey = 'app1'

export default {
  data() {
    return {
      interstitial: undefined,
    }
  },
  mounted() {
    const interstitial = this.$refs['interstitial']
    this.interstitial = new AD.interstitialAD(interstitial, { appkey });
  },
}
```

