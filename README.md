# Logseq 复制页面路径插件

一键复制当前页面的本地文件路径到剪贴板。

![image-20260129233950983](C:\Users\ZhuanZ\AppData\Roaming\Typora\typora-user-images\image-20260129233950983.png)

![image-20260129234011709](C:\Users\ZhuanZ\AppData\Roaming\Typora\typora-user-images\image-20260129234011709.png)

## 功能特点

- ✅ 复制页面的绝对路径
- ✅ 复制页面的相对路径
- ✅ 复制为 `file://` 协议链接
- ✅ 复制为 Markdown 链接格式
- ✅ 支持斜杠命令 `/copy`
- ✅ 支持工具栏按钮
- ✅ 支持快捷键 `Ctrl/Cmd + Shift + P`

## 安装方法

### 方法一：从插件市场安装（推荐）

等待插件上架后，在 Logseq 插件市场搜索 "复制页面路径" 并安装。

### 方法二：手动安装

1. 下载本插件文件夹
2. 打开 Logseq，点击右上角 `···` → `插件`
3. 点击 `加载已解压的插件`
4. 选择本插件文件夹
5. 启用插件

### 方法三：使用 Git

```bash
# 将插件克隆到 Logseq 插件目录
cd ~/.logseq/plugins  # macOS/Linux
cd %USERPROFILE%\.logseq\plugins  # Windows
git clone [插件地址] logseq-plugin-copy-page-path
```

## 使用方法

### 1. 斜杠命令

在编辑器中输入 `/copy`，选择以下命令：

| 命令 | 说明 |
|------|------|
| `/copy page path` | 复制绝对路径 |
| `/copy page relative path` | 复制相对路径 |
| `/copy page file link` | 复制 file:// 链接 |
| `/copy page markdown link` | 复制 Markdown 格式链接 |

### 2. 工具栏按钮

点击右上角工具栏的 🔗 图标，快速复制当前页面的绝对路径。

### 3. 快捷键

- 可以设置

## 使用示例

假设你的图形目录为 `C:\Users\Name\Documents\Logseq`，当前页面为 `项目管理`：

| 复制类型 | 结果 |
|---------|------|
| 绝对路径 | `C:\Users\Name\Documents\Logseq\pages\项目管理.md` |
| 相对路径 | `./pages/项目管理.md` |
| file:// 链接 | `file://C:\Users\Name\Documents\Logseq\pages\项目管理.md` |
| Markdown 链接 | `[项目管理](./pages/项目管理.md)` |

## 支持的页面类型

- ✅ 普通页面 (pages/)
- ✅ 日志页面 (journals/)
- ✅ 命名空间页面 (pages/namespace%2Fpage.md)

## 注意事项

1. 插件需要访问图形的文件系统路径，请确保图形已正确加载
2. 页面名称中的非法字符会被替换为下划线 `_`
3. 如果复制失败，请检查浏览器/应用是否允许访问剪贴板
3. 页面需要有内容，有内容的话才会产生markdown，才能够复制这个markdown的地址

## 兼容性

- Logseq 0.9.x 及以上版本
- 支持 Windows、macOS、Linux
- 支持桌面端和 Web 端（Web 端部分功能受限）



## 问题反馈

如有问题或建议，请在 GitHub Issues 中反馈。

## 许可证

MIT License

---

**Enjoy!** 🚀
