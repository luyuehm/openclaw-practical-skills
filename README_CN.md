# openclaw-practical-skills

一个统一、实用的 OpenClaw Skills 开源集合。

## 这个仓库提供什么

- `self-healing`：回归/波动问题的标准化自愈流程
- `release-readiness`：发布前可证据化的 PASS/FAIL 验收
- `lesson-extractor`：把事故经验沉淀为可复用规则

## 目录结构

```text
skills/
  self-healing/
    SKILL.md
  release-readiness/
    SKILL.md
  lesson-extractor/
    SKILL.md
templates/
  pr-summary.md
README.md
README_CN.md
LICENSE
```

## 快速开始

1. 将 skills 目录复制到你的 agent 工作区
2. 按项目上下文触发对应 skill
3. 输出坚持“短、可审计、有证据”

## 推荐使用顺序

1. 先用 **self-healing** 解决问题
2. 再用 **release-readiness** 做发布门禁
3. 最后用 **lesson-extractor** 沉淀经验

## 贡献规范

- 一个 skill 只做一类事
- 必须有标准输出模板
- 优先命令和客观检查，不靠主观描述
- 边界场景要给例子

## 许可证

MIT
