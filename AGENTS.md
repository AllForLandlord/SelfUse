# AllForLandlord 项目协作说明

## 仓库结构

- 本目录是独立的 Git 仓库 `SelfUse`。
- Clash/Mihomo 规则文件位于 `Clash` 目录。
- `Mihomo-Yaml` 是同级的另一个独立 Git 仓库，其配置通过 `rule-providers` 引用本仓库中的规则文件。

## Mihomo 配置约定

- 配置按 Mihomo 内核语法维护，优先参考官方文档：
  - https://github.com/MetaCubeX/mihomo/blob/Meta/docs/config.yaml
  - https://wiki.metacubex.one/config/proxy-providers/
  - https://wiki.metacubex.one/config/proxy-groups/
  - https://wiki.metacubex.one/config/rules/
  - https://wiki.metacubex.one/config/rule-providers/
- 修改规则文件前先确认目标仓库状态；完成后检查 diff 和内容格式。
- 不要在输出、提交说明或新文档中泄露节点密码、订阅地址中的敏感信息或 `PASS-INFO` 内容。

## Git 操作

- 只修改用户明确指定的文件和范围。
- 提交前确认没有混入无关改动；推送到对应仓库的 `main` 分支。
- 删除文件必须是用户明确指定的单个文件，不得批量删除或删除目录。

