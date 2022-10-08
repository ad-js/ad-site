---
page: false
title: AD.js 横幅广告
footer: false
---

# 横幅广告


## 示例
<script setup>
import Banner from '@theme/examplate/banner.vue'
</script>

<Banner />

## CDN
```html
  <div id="ad-banner1" style="background-color: red;float: right; width:100vw;height:10vw;"></div>

```

```js
  <script src="../../../dist/ad.js"></script>
  // 创建容器
  const banner1 = document.getElementById('ad-banner1')
  // 初始化
  new AD.BannerAD(banner1, { appkey });
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
    const banner = this.$refs['banner']
    this.banner = new AD.BannerAD(banner, { appkey });
  },
}
```

