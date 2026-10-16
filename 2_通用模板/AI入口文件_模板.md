# 各 AI 的入口文件（模板）

每个 AI 开工时都会读自己的入口文件。入口里只写"去读共用的三份规矩"，规矩本身只维护一份。把下面的内容分别存到对应的位置，`你的用户名` 换成自己 Mac 的用户名。

## Claude Code → `~/.claude/CLAUDE.md`

```markdown
# 给 Claude Code 的说明（全局）

这台电脑上的 AI 共用一套规矩，这里只放入口。

- 个人说明：@~/.codex/AGENTS.md
- AI 协作手册：@~/Documents/4_AI工具/AI协作手册.md
- 文稿里东西放哪：@~/Documents/文稿分类说明.md
```

## WorkBuddy → `~/.workbuddy/CODEBUDDY.md`

WorkBuddy 也支持 `@` 引用，用完整路径最稳：

```markdown
# 给 WorkBuddy 的说明（全局）

- 个人说明：@/Users/你的用户名/.codex/AGENTS.md
- AI 协作手册：@/Users/你的用户名/Documents/4_AI工具/AI协作手册.md
- 文稿里东西放哪：@/Users/你的用户名/Documents/文稿分类说明.md
```

## Codex → `~/.codex/AGENTS.md`

Codex 直接读这份文件，它本身就是个人说明的正本（见「个人说明_模板」）。末尾的「AI 工具协作」一节写明另外两份规矩在哪。

## Gemini / Antigravity → `~/.gemini/GEMINI.md`

Gemini 出于安全限制，只能引用项目里的文件，引用不了上面三份。所以这里放一份**摘要**，开头写明"完整版以三份正本为准"，正本改了要顺手同步这份摘要。摘要至少包括：你是谁、怎么沟通；文件放哪的首页结构；绝对不能动的路径；下载放哪的规矩；只听你指挥去问别的 AI。

## 怎么验证生效了

分别问每个 AI 一个只有读过规矩才答得上来的问题，比如"AI 协作手册在哪个路径？""WorkBuddy 的工程该放哪？"。答对了就说明接上了。
