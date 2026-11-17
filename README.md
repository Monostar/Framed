# Framed

为照片添加精致边框与裁切拼图的桌面工具。纯本地处理，不上传任何照片。

## 功能

- 画布比例：1:1 / 3:2 / 2:3 / 4:3 / 5:4 / 16:9 / 16:10 / 65:24，横竖屏切换
- 边框：宽度、圆角、颜色可调
- 照片位置：水平 / 垂直偏移
- 背景：纯色 / 照片模糊（含平均色 + 主体色一键取色）
- 裁切拼图：把一张图平均切成 2 / 3 / 4 张，社交平台滑动拼接
- 输出：自定义长边、PNG / JPEG / WebP、质量、目标文件大小
- 批量：多选上传、缩略图切换、一键导出全部

## 下载

前往 [Releases](https://github.com/你的用户名/Framed/releases) 页面，根据系统下载：

- **macOS**：`Framed.dmg`
- **Windows**：`Framed.msi`（安装包）或 `Framed.exe`（免安装）

### macOS 首次打开说明

应用未经过 Apple 签名，首次打开时系统会提示"无法验证开发者"。解决方法：

1. 右键点击 `Framed.app` → 选"打开"
2. 或在「系统设置 → 隐私与安全性」里点击"仍要打开"

### Windows 首次打开说明

如果 SmartScreen 弹出"未知发布者"提示：

1. 点"更多信息"
2. 点"仍要运行"

## 开发

```bash
# 安装依赖
npm install -g pake-cli

# 本地运行
pake ./src/framed.html --name "Framed" --debug

# 本地打包
pake ./src/framed.html --name "Framed" --keep-binary