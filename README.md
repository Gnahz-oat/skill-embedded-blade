# 嵌入式之刃 / Embedded Blade

Codex skill：用于嵌入式软件、固件和驱动任务。先依据实际源码和配置分析，报告修改方案；获明确授权后执行最小修改、工程清理和验证。

安装目录：`~/.codex/skills/embedded-blade/`。中文显示名“嵌入式之刃”，英文名 **Embedded Blade**，调用标识 `$embedded-blade`。按任务描述自动匹配已启用。

GitHub 仓库地址保留 `Gnahz-oat/skill-embedded-person`，避免已有链接失效；技能名称、安装目录和调用名已迁移到 `embedded-blade`。从仓库根目录安装时指定新名称：

```sh
python <skill-installer目录>/scripts/install-skill-from-github.py --repo Gnahz-oat/skill-embedded-person --path . --name embedded-blade
```

旧版升级：先检查并保存旧安装的本地改动，再安装新版；替换全局指令中的旧路径与 `$embedded-person`。确认新版有效后移出旧安装目录，避免同时启用两套规则。不要覆盖现有工程文件或自动改动其他项目的指令。

新功能开发：先只读检查实现，再澄清影响行为的关键问题；信息足够时给出逐文件方案和风险，等待修改授权。已有明确授权在其范围内持续有效。

项目接续：沿用项目现有本地进度文件；没有约定时使用根目录 `CODEX_PROGRESS.md`。新聊天先读，再核对源码和配置；获批改动后更新当前状态及验证结果。Git 项目通过仓库本地排除规则避免提交进度文件，首次创建列入修改方案。

工程清理：每次修改后遍历整个当前工程及 Markdown；连续编辑可在批次结束统一检查。用户已常设授权删除所有经核实失效或无用的工程文件，并更新或删除过期的当前说明。核查构建、运行、脚本、资源和文档引用；用途未确认的文件继续调查并报告。保护用户已有改动、有效依赖和有追溯用途的原始/历史记录，不把无搜索命中直接当作无用。清理后验证并留下精简记录，不扩展功能修改权限。

维护时同步修改 `SKILL.md`、`agents/openai.yaml` 和本说明，并同步本地安装。详细执行规则以 `SKILL.md` 为准。
