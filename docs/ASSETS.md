# 头像和背景图说明

## 头像

- 位置：`src/assets/images/demo-avatar.png`
- 也可以在 `src/config.ts` 里改 `profileConfig.avatar`
- 推荐格式：`PNG` / `JPG` / `WebP`
- 推荐尺寸：`512x512` 或 `1024x1024`
- 推荐比例：`1:1`
- 建议大小：尽量控制在 `500KB` 左右或更小

## 页面背景图

- 位置：`src/assets/images/demo-banner.png`
- 也可以在 `src/config.ts` 里改 `siteConfig.banner.src`
- 推荐格式：`JPG` / `WebP`
- 推荐比例：横图，优先 `16:9` 或 `21:9`
- 推荐尺寸：`1920x720`、`2400x900`、`2560x960`
- 建议大小：单张尽量控制在 `1MB` 以内

## 多张背景图随机切换

当前代码已经支持。

做法是：

1. 把多张背景图放到 `public/images/banners/`
2. 在 `src/config.ts` 的 `siteConfig.banner.srcList` 里填写这些公开路径
3. 刷新页面时会随机挑一张作为首页背景

示例：

```ts
banner: {
  enable: true,
  src: "assets/images/demo-banner.png",
  srcList: [
    "/images/banners/a.jpg",
    "/images/banners/b.jpg",
    "/images/banners/c.jpg",
  ],
  position: "center",
  credit: { enable: false, text: "", url: "" },
}
```

如果你只想固定一张背景图，把 `srcList` 留空就行。
