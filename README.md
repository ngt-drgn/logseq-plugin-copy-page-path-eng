# Logseq Copy Page Path Plugin

One-click copy of the current page's local file path to the clipboard.

![image-20260129233950983](C:\Users\ZhuanZ\AppData\Roaming\Typora\typora-user-images\image-20260129233950983.png)

![image-20260129234011709](C:\Users\ZhuanZ\AppData\Roaming\Typora\typora-user-images\image-20260129234011709.png)

## Features

- ✅ Copy the page's absolute path
- ✅ Copy the page's relative path
- ✅ Copy as a `file://` protocol link
- ✅ Copy as a Markdown link
- ✅ Supports slash command `/copy`
- ✅ Supports toolbar button
- ✅ Supports shortcut `Ctrl/Cmd + Shift + P`

## Installation

### Method 1: Install from the plugin marketplace (recommended)

Once the plugin is listed in the marketplace, search for "Copy Page Path" in the Logseq plugin market and install it.

### Method 2: Manual installation

1. Download this plugin folder
2. Open Logseq, click the top-right `···` → `Plugins`
3. Click `Load unpacked plugin`
4. Select this plugin folder
5. Enable the plugin

### Method 3: Using Git

```bash
# Clone the plugin into the Logseq plugins directory
d = ~/.logseq/plugins  # macOS/Linux
cd %USERPROFILE%\.logseq\plugins  # Windows
git clone [plugin URL] logseq-plugin-copy-page-path
```

## Usage

### 1. Slash command

In the editor, type `/copy` and choose one of the following commands:

| Command | Description |
|--------|-------------|
| `/copy page path` | Copy absolute path |
| `/copy page relative path` | Copy relative path |
| `/copy page file link` | Copy `file://` link |
| `/copy page markdown link` | Copy Markdown link |

### 2. Toolbar button

Click the 🔗 icon in the top-right toolbar to quickly copy the current page's absolute path.

### 3. Shortcut key

- Can be configured

## Example

Assume your graph directory is `C:\Users\Name\Documents\Logseq` and the current page is `Project Management`:

| Copy type | Result |
|-----------|--------|
| Absolute path | `C:\Users\Name\Documents\Logseq\pages\Project Management.md` |
| Relative path | `./pages/Project Management.md` |
| `file://` link | `file://C:\Users\Name\Documents\Logseq\pages\Project Management.md` |
| Markdown link | `[Project Management](./pages/Project Management.md)` |

## Supported page types

- ✅ Regular pages (`pages/`)
- ✅ Journal pages (`journals/`)
- ✅ Namespaced pages (`pages/namespace%2Fpage.md`)

## Notes

1. The plugin needs access to the graph's file system path; make sure the graph is loaded correctly.
2. Illegal characters in page names will be replaced with underscores `_`.
3. If copying fails, check whether the browser/app is allowed to access the clipboard.
4. A page must contain content; only then can a Markdown link be generated and copied.

## Compatibility

- Logseq 0.9.x and above
- Supports Windows, macOS, and Linux
- Supports desktop and web versions (some features are limited on the web version)

## Feedback

If you have any issues or suggestions, please report them in GitHub Issues.

## License

MIT License

---

**Enjoy!** 🚀
