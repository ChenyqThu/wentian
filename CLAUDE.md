# CLAUDE.md — 问天.skill

## 项目概述

问天是一个 AI 智囊团技能（Skill），将各领域顶级思考者的认知方式蒸馏为可调用的专家 Skill。

## 目录结构

```
wentian/
├── SKILL.md                # 主技能：模式分发 + 咨询路由 + 蒸馏入口
├── expert-registry.md      # 专家注册表（YAML），路由匹配用
├── experts/{id}/SKILL.md   # 各专家的认知 Skill（仓颉 v2 格式）
├── experts/{id}/references/research/  # 蒸馏参考素材
├── templates/
│   ├── expert-template.md      # 仓颉 v2 专家模板
│   └── distillation-guide.md   # 7 步蒸馏流程指南
└── references/             # 通用参考资料
```

## 两种模式

### 咨询模式
读取 `SKILL.md` 中的路由逻辑，根据用户问题匹配 `expert-registry.md` 中的专家，加载对应 `experts/{id}/SKILL.md` 回答。支持单专家和圆桌（2-3人）模式。

### 蒸馏模式
按 `templates/distillation-guide.md` 的 7 步流程，从素材中提取认知上下文，生成新专家 SKILL.md 并注册。

## 新增专家流程

1. 准备素材（上传文件或指定人名由 AI 网搜）
2. 触发蒸馏模式：「蒸馏XX」「创建专家」
3. 自动按 7 步流程执行，产出写入 `experts/{id}/SKILL.md`
4. 自动更新 `expert-registry.md`

手动新增：
1. 按 `templates/expert-template.md` 编写 `experts/{id}/SKILL.md`
2. 在 `expert-registry.md` 末尾追加条目
3. 将蒸馏素材放入 `experts/{id}/references/research/`

## 专家格式：仓颉 v2（认知植入）

核心原则：不给模型写推理流程，只注入模型不可能自己知道的认知上下文。

必须包含：
- 信念及其形成故事（每条信念必须有"为什么信"）
- 真实决策案例 + 事后反思
- 自认的失败教训
- 内在矛盾（保留不调和）
- 认知边界
- 全部第一人称

禁止：
- Step 1/2/3 推理步骤
- 通用金句（无形成故事的不入）
- 详细表达规则（3 偏好 + 3 禁忌即可）

## 质量标准

蒸馏后 9 项自检：
1. 每条信念都有形成故事
2. 每个决策都有事后反思
3. 失败全部是本人承认的
4. 矛盾是真实存在的
5. 认知边界 >= 3 条
6. 没有通用金句
7. 没有推理步骤
8. 表达 DNA <= 3+3
9. 素材有保存

## 编辑规范

- 专家 SKILL.md 文件名统一为 `SKILL.md`，放在 `experts/{id}/` 下
- id 使用 kebab-case（如 `zhang-yiming`、`paul-graham`）
- 注册表中 trigger_keywords 和 avoid 要准确，影响路由质量
- 参考素材放 `experts/{id}/references/research/`，不要放原始大文件
