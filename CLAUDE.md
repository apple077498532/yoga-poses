# Yoga Poses

## 路径
- 代码：`~/Documents/Jeffcode/yoga-poses/`
- Obsidian：`~/Documents/obsidian/jeffmindfulness/Yoga/`

## 文件
- `poses.json` — 体式数据（核心）
- `index.html` — 网页排序工具（单文件，无 build）
- `svg/` — 小人图（第二阶段）

## poses.json Schema
```json
{
  "id": "tadasana",
  "sanskrit": "Tāḍāsana",
  "chinese": "山式",
  "english": "Mountain Pose",
  "aliases": ["Samasthiti"],
  "category": "standing",
  "tags": ["beginner"],
  "svg": null
}
```

## Category
standing, seated, supine, prone, inversion, balance, twist, backbend, forward-fold, arm-balance

## 规则
- `id` 唯一，梵语小写 slug
- 新增前先查重（id / sanskrit）
- Sanskrit 用正确音标（ā ī ū ś ṣ ṇ）
- tags 含难度：beginner / intermediate / advanced
- 改完自动 commit + push
- 笔记类内容存 Obsidian Yoga/ 目录
