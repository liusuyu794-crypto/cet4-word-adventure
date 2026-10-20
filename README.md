# 四级单词冒险（CET-4 Vocabulary Quest）

一个纯静态网页英语四级词汇闯关游戏，适配电脑和手机，不需要安装依赖或构建工具。

## 功能
- 闯关选择释义、单词卡、错词复习、词典搜索
- 经验值、已掌握词条、每日答对数量与每日目标
- 英式 / 美式浏览器语音合成切换
- 使用 localStorage 在当前浏览器保存学习进度
- 导出学习记录 JSON
- 优先载入公开 CET-4 词表，按 headword 去重；在线词表不可用时切换到内置演示词

## 发布到 GitHub Pages（免费固定网址）

1. 登录 GitHub 并创建一个新的 **Public** repository，例如 `cet4-word-adventure`。
2. 将本目录中的 `index.html` 和 `README.md` 上传到仓库根目录并提交。
3. 打开仓库 **Settings → Pages**。
4. 在 **Build and deployment** 中选择 **Deploy from a branch**。
5. Branch 选择 `main`，目录选择 `/(root)`，点击 **Save**。
6. 等待 GitHub Pages 完成部署。页面会显示网址，通常形如：
   `https://你的GitHub用户名.github.io/cet4-word-adventure/`
7. 将该网址加入浏览器书签，即可随时访问。手机也可以打开；iPhone Safari 或 Android Chrome 可使用“添加到主屏幕”。

如果仓库名是 `你的用户名.github.io`，网址通常是 `https://你的用户名.github.io/`。

## 词库与发音说明

- 在线词库来源：`mahavivo/english-wordlists` 的 `CET4_edited.txt`，项目说明该表包含约 4615 个词条：
  https://github.com/mahavivo/english-wordlists
- 页面运行时从 GitHub Raw / jsDelivr 获取词表，因此首次完整载入需要网络。若两处词库源都无法访问，会显示内置演示词汇，不会假装已载入全部词表。
- 词表中提供的音标沿用来源数据；英美口音切换作用于浏览器语音合成，实际声音由设备和浏览器已安装的语音决定，不保证每台设备都同时具有高质量英式和美式语音。
- 学习进度保存于当前浏览器的 localStorage。换设备或清除浏览器数据不会自动同步；可使用“导出学习记录”备份。
- 此词表为公开学习资源整理，不代表官方考试机构发布的唯一、最新大纲。不同词表的统计口径可能不同，应用会显示实际载入并去重后的词条数量。

## 本地预览

直接双击 `index.html` 通常也能打开；为确保浏览器网络请求正常，推荐使用静态网页托管（GitHub Pages）或本地静态服务器。
