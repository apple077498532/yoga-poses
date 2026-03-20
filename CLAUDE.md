# Yoga Poses 项目指引

## 仓库结构
- `poses.json` — 体式资料库（核心数据）
- `index.html` — 网页排序工具（单文件，无 build）
- `svg/` — 小人图 SVG（第二阶段）

## poses.json Schema
```json
{
  "id": "tadasana",           // 梵语小写 slug，唯一标识
  "sanskrit": "Tāḍāsana",    // 带音标的梵语名
  "chinese": "山式",           // 中文名
  "english": "Mountain Pose",  // 英文名
  "aliases": ["Samasthiti"],   // 别名
  "category": "standing",      // 分类（见下方）
  "tags": ["beginner"],        // 标签
  "svg": null                  // SVG 文件路径或 null
}
```

## Category 固定集合
standing, seated, supine, prone, inversion, balance, twist, backbend, forward-fold, arm-balance

## 规则
- `id` 必须唯一，使用梵语小写 slug
- 新增体式前先检查是否已存在（搜 id 或 sanskrit）
- Sanskrit 名使用正确的音标符号（ā, ī, ū, ś, ṣ, ṇ 等）
- 中文名尽量使用通用翻译
- tags 包含难度：beginner / intermediate / advanced
