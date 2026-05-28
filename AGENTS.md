# AGENTS.md

## 这个项目是什么

这是一个小游戏项目。这里的游戏主要给小朋友练习单词、字母和反应。

现在有这些游戏：

- `word-spelling-practice/word-spelling-practice.html`
- `word-spelling-practice-duck/word-spelling-practice-duck.html`
- `duck-letter-hop/duck-letter-hop.html`

每个游戏基本都是一个单独的 HTML 文件。打开文件就能玩，不需要安装复杂工具。

## 写代码时要记住

- 每个小游戏尽量放在自己的文件夹里。
- 不要随便把一个游戏的代码改到另一个游戏里。
- 页面上的文字要保持中文、简单、亲切。
- 游戏要适合手机和电脑屏幕。
- 按钮、分数、进度条这些东西不要乱跳位置。
- 尽量用普通的 HTML、CSS 和 JavaScript。
- 不要随便加入新的第三方库，除非用户明确要求。
- 只改用户要改的地方，不要顺手大改一堆无关内容。

## 新游戏怎么放

- 新游戏放在新的顶层文件夹里。
- 文件夹名和 HTML 文件名尽量一样。
- 例子：`my-game/my-game.html`
- 如果游戏以后有图片、声音或其他文件，也放在这个游戏自己的文件夹里。

## 怎么检查游戏

这个项目没有自动测试。改完以后，要自己打开浏览器检查。

可以直接打开 HTML 文件，也可以在项目根目录运行：

```sh
python3 -m http.server 8000
```

然后在浏览器里打开：

- `http://localhost:8000/word-spelling-practice/word-spelling-practice.html`
- `http://localhost:8000/word-spelling-practice-duck/word-spelling-practice-duck.html`
- `http://localhost:8000/duck-letter-hop/duck-letter-hop.html`

检查时要看这些：

- 第一眼打开，画面是不是正常。
- 手机大小和电脑大小都要看一看。
- 按钮能不能点。
- 键盘操作能不能用。
- 分数、生命、进度、倒计时有没有正常变化。
- 游戏结束、过关、失败这些状态有没有正常出现。
- 文字有没有挤在一起、跑出去或盖住别的东西。
- 如果有声音或朗读功能，不能用的时候也不要让游戏坏掉。

## 写代码的小习惯

- 变量和函数名字要清楚，看名字就知道大概在做什么。
- 默认用 `const`，真的需要改值时再用 `let`。
- 颜色尽量放在 CSS 顶部的变量里，方便以后一起改。
- 注释不用写太多，只在代码不容易看懂时加一点说明。
- 不要为了显得高级，把简单事情写复杂。

## Git 规则

- 改文件前先看 `git status --short`。
- 不要撤销别人已经改过的内容，除非用户明确说可以。
- 每次提交只放相关改动，不要把无关东西混在一起。
- 每次 commit 的说明要用简单中文写，尽量让小朋友也能看懂这次改了什么。
- Codex 每次改完代码并检查通过后，要自动提交 commit，并推送 push 到当前分支。
