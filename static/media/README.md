# 背景图片使用说明

## 如何添加背景图片

1. **添加图片文件**：
   - 将你的背景图片放在 `static/media/` 目录下
   - 支持的格式：JPG, PNG, WebP
   - 建议尺寸：1920x1080 或更高分辨率

2. **修改配置**：
   在 `content/_index.md` 中，将：
   ```yaml
   design:
     css_class: hbx-bg-gradient
   ```
   
   改为：
   ```yaml
   design:
     background:
       image: "media/your-image-name.jpg"
   ```

## 示例配置

```yaml
design:
  # 使用背景图片
  background:
    image: "media/background.jpg"
  
  # 或者使用渐变背景
  # css_class: hbx-bg-gradient
```

## 图片建议

- 使用高质量、高分辨率的图片
- 避免过于复杂的图片，确保文字可读性
- 考虑使用淡色或模糊的背景图片
- 图片会自动添加半透明遮罩层以提高文字可读性
