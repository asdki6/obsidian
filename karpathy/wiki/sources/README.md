# wiki/sources/ — 来源摘要

每当你（LLM）摄入一个 `karpathy/raw/` 中的原始来源，在此创建对应的摘要页。

## 命名规范
`来源_文章标题.md`

## Frontmatter
```yaml
type: source
tags: [...]
summary: "一句话摘要"
sources: ["karpathy/raw/articles/ai/xxx.md"]
```

## 内容结构
1. 来源信息（标题、作者、日期、链接、原始文件路径）
2. 核心要点（3-7 条）
3. 关键引文
4. 关联实体 → `[[../entities/实体_xxx]]`
5. 关联概念 → `[[../concepts/概念_xxx]]`
