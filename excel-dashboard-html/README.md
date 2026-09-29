# Excel Dashboard HTML

将 Excel 数据转换为可筛选、切换、比较和查看明细的交互式 HTML 数据看板。

这个 skill 的重点不是读取 Excel 后直接堆图表，而是先判断：

1. 用户想通过数据看什么
2. 数据里什么值得看
3. 这些数据应该怎么呈现
4. 再生成可直接运行的独立 HTML Dashboard

## 适用场景

- 从 Excel 工作簿生成经营分析、内容运营、销售、社群、目标完成等数据看板
- 需要先识别增长、下降、异常和待查问题，再选择合适图表
- 需要生成具有设计感、动态图表、筛选和页面切换的 HTML Dashboard

## 主要能力

- 读取并理解 Excel 的 Sheet、字段、时间、分类、数值和指标关系
- 在生成前确认分析目的和页面形式
- 支持纵向滚动单页，也支持导航切换多个横向页面
- 使用真实数据生成 3 个首页视觉预览，帮助选择风格
- 融合 Frontend Slides 的视觉探索方法，但输出是 Dashboard，不是幻灯片
- 支持 KPI、折线图、柱状图、饼图、环形图、进度条、表格和详情面板
- 图表带有合适的动态增长、绘制、填充和 count up 效果
- 多页面桌面端优先一页一屏，默认使用顶部导航，避免侧边导航占用数据空间
- 数据较少的页面会用均衡布局和有依据的小图表减少大片空白
- 自定义鼠标光圈替代系统指针，避免双指针

## 安装

将本目录复制到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R excel-dashboard-html ~/.codex/skills/
```

安装后可以这样调用：

```text
用 $excel-dashboard-html，把这份 Excel 做成交互式数据看板
```

## 文件结构

```text
excel-dashboard-html/
├── SKILL.md
├── README.md
└── agents/
    └── openai.yaml
```

## 上传 GitHub 前检查

```bash
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py excel-dashboard-html
```

如果输出 `Skill is valid!`，说明 skill 的基础结构有效.
