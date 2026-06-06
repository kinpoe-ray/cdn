# CDN

Public image hosting via GitHub raw URLs. Primarily used for:

- 微信公众号封面图（wechat-cover skill 生成）
- 文章配图
- 其他需要外链访问的静态资源

## 目录结构

```
covers/
├── YYYYMMDD/
│   ├── {theme}_horizontal_{date}_{slug}.png   # 横图 2.35:1
│   ├── {theme}_square_{date}_{slug}.png       # 方图 1:1
│   └── ...
└── ...
```

## 命名规范

- 格式：`{theme}_{orientation}_{YYYYMMDD}_{slug}.png`
- theme: `kami` / `indigo` / `tech`
- orientation: `horizontal` (2.35:1) / `square` (1:1)

## 使用方式

图片通过 GitHub raw URL 直接引用：

```
https://raw.githubusercontent.com/kinpoe-ray/cdn/main/covers/20260503/kami_horizontal_20260503_harness.png
```

> ⚠️ 本仓库由自动化工具（wechat-cover skill）管理，一般不需要手动上传。
