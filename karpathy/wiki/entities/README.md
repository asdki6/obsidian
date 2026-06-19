# wiki/entities/ — 实体页

跨来源积累的实体信息：人物、书籍、项目、组织、工具等。

## 命名规范
`实体_名称.md`

## 何时创建/更新
- 来源中提到新人物/书籍/工具 → Ingest 时创建
- 新来源触及已有实体 → 追加更新，不覆盖

## Frontmatter
```yaml
type: entity
tags: [...]
summary: "一句话描述"
sources: ["karpathy/wiki/sources/来源_xxx.md"]
```

## 内容结构
1. 基本信息（类型、别名、链接）
2. 特征/属性
3. 关键事件/作品
4. 关联来源
5. 关联概念
