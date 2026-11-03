# 通用代理软件图标库

支持 **Quantumult X / Loon / Surge** 等代理软件的远程图标订阅。

## 订阅地址

| 用途 | 地址 |
|------|------|
| QX 图标订阅 | `https://raw.githubusercontent.com/roamout/icon-library/main/icon.json` |

## 使用方式

### Quantumult X
1. 打开 Quantumult X → 设置 → 图标订阅（或「资源解析器」添加订阅）
2. 填入上面的订阅地址
3. 刷新后即可在策略组 / 节点选择对应图标

### Loon / Surge
直接引用单个图标地址，例如：
```
icon = https://raw.githubusercontent.com/roamout/icon-library/main/icons/google.png
```

## 目录结构

```
icon-library/
├── icon.json        # QX 图标订阅文件
├── icons/           # 图标文件（png / 建议 108x108 或 144x144）
└── README.md
```

## 添加图标

1. 将图标文件放入 `icons/` 目录（建议使用 PNG，尺寸 108×108 或 144×144）
2. 在 `icon.json` 的 `icons` 数组中新增一项：
```json
{ "name": "图标名称", "url": "https://raw.githubusercontent.com/roamout/icon-library/main/icons/文件名.png" }
```
3. 提交推送后，订阅端刷新即可生效

## 注意

- 图标请使用自有或可自由分发（如品牌官方公开资源）的图片，注意版权
- GitHub raw 地址会自动跳转到 CDN，订阅端一般可正常访问
