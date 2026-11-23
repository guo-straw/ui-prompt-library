# 待整理收集区（inbox）

新收集的 UI 提示词先放这里，注明来源和日期；整理（去重、定分类、补中文说明）后移入 prompts.json，并从这里删掉。

<!-- 格式：
## YYYY-MM-DD · 来源（一句话）
- 原文/链接：
- 初步分类：
- 备注：
-->

## 2026-11-17 · 抖音 @费纸张《5个小细节让AI设计的界面看着更舒服》
- 原文/链接：https://v.douyin.com/rL3vWzup154/（短链实际作品 id 7699104647889423667（用户消息里的直链 7695264996816620863 是另一个作品：SpicyTater《用大白话向AI描述后台菜单交互Skill》，与本条无关））
- 状态：2026-11-17 已核对（未登录、关闭弹窗后观看）：费纸张《AI设计技巧分享》第3集，2026-10-21 发布，42 秒。5 个细节已核实：①等宽数字 tabular-nums ②同心圆角 外层=内层+内边距 ③错开入场（片尾汇总间隔100ms）④平衡标题换行 text-wrap: balance ⑤阴影代替边框（多层柔和 box-shadow）。完整旁白未转录成功，要点以画面文字/字幕片段/文案为准；第5条阴影完整代码值未在画面中完全显示。
- 已处理：先原创收集「细节优化」类 10 条；核对后已补入原作版 5 条（合集1 + 等宽数字/同心圆角/错开入场/平衡换行 4 条单项，阴影代替边框与已有 detail-shadow-border 同主题、合集条目内含原作版表述）。本条目留档，不再待办。

## 2026-11-17 · 公开渠道收集（Questera / Superdesign / TemplatesCenter）
- 原文/链接：https://www.questera.ai/blogs/ai-prompts-beautiful-ui-designs（Bento 网格、瑞士极简模板，已打开核对）；https://superdesign.dev/blog/ui-design-prompts（定价页、设置页主从布局模板，已打开核对）；https://www.templatescenter.com/blogs/liquid-glass-ui-prompts-20-templates-that-work（液态玻璃五要素配方，已打开核对）
- 状态：2026-11-17 已核对上述三页正文，按统一格式改写整理，非逐字摘录；与现有 33 条去重（避开已有粗野主义、杂志编辑风、Linear 后台等同场景同风格条目）。
- 已处理：新增 5 条 — 其中 landing-bento-grid、saas-settings-master-detail 已移入 prompts.json；其余 3 条（landing-swiss-minimal、landing-pricing-saas、detail-liquid-glass）于 2026-11-20 本轮验证通过后移入 prompts.json 与对应分类 md。本条目留档，不再待办。

## 待验证区（2026-11-17 起执行新规：验证通过才进正式库）

以下条目已收集整理但尚未生成验证，暂存于此；逐条生成验证通过后才移入 prompts.json 并提交。

### 空间收集轮次新增（2026-11-17，同样待验证）

## 2026-11-17 晚 · 费纸张主页系统收集（用户登录抖音后逐条核对）

来源：费纸张抖音主页（抖音号 67394924732），作品 20 条，其中 17 条与 AI 设计/UI 相关，已逐条打开核对；3 条无关（Agent 省钱指南、实测 DeepSeek Flash 做视频、《看不见的城市》）只记标题跳过。用户已关注费纸张并授权持续收集其视频内容。

### 核心条目原文：第6集《四条规则去掉设计里的 AI 味儿》（2026-11-03，作品 7703624707744091446）

片尾提示词框（## 视觉规则）原文：配色：中性色为主，用明暗对比突出主要操作。强调色可选，最多一种。禁用渐变、发光和彩色阴影。／间距：仅用 4 8 12 16 24 32 px。组内间距小于组间间距。／圆角：仅用 6 10 16 px。嵌套圆角：外圆角 = 内圆角 + 内边距。／对齐：同一列元素共用左边缘。另第四条字幕：删掉表情符号、感叹号和装饰徽章。（评论区 WINDQIIIII 的「统一线性图标」是评论者补充，非视频原文，未计入。）

### 第3集《5个小细节》复核补充参数（作品 7699104647889423667）

等宽数字 font-variant-numeric: tabular-nums；同心圆角示例：外层 36 = 内层 20 + 内边距 16，border-radius: calc(20px + 16px)；错开入场时间轴 0 / 400ms / 800ms / 1.2s；平衡换行 h1 { text-wrap: balance; }；阴影代边框 box-shadow: 0 0 1px rgb(0 0 0 / .06), 0 1px 2px -1px rgb(0 0 0 / .06), 0 2px 4px rgb(0 0 0 / .04)。待验证区对应单条验证时按此参数核对。

### 只记录不立条目的两条

- 热成像文字特效（7694648035741044002）：44 行 SVG 滤镜代码画面字号过小未逐行抄录（节点含 feGaussianBlur/feColorMatrix/feBlend 等），无法忠实还原，不立条目。

- 一分钟入门字体设计（7694513054695869723）：字体分类知识（衬线/无衬线/几何/人文等），非生成提示词，只作知识记录，不立条目。

- 文字随音乐变色动效（7699531773557869865）：属产品发布视频文字动画，非 UI 提示词，不立条目。

### 本批新增待验证条目（13 条）




## 2026-11-17 夜 · SpicyTater 主页系统收集（用户指示关注并收集）

作者：SpicyTater（抖音号 xinxinyaokuaileo，湖南，独立开发者），作品 62 条，设计相关 38 条；已关注（粉丝 6056→6057）。其第22集《后台菜单交互》即 2026-11-17 用户最早分享的那条链接（7695264996816620863）。

**重要局限**：本次浏览器里视频无法播放（播放器一直 00:00 加载），要点来自页面文案 + 抖音「章节要点」AI 摘要，**不是视频逐字原文**；条目已在 source 里如实标注「章节摘录」。8 条无章节要点且文案为模板/错贴，未能提取：Vibe 第33集（查数据）、第27集粒子交互、第23集高级布局、第19集编辑工具、第18集任务反馈、第17集标题动效、第8集图表动画、第4集展开面板——只在来源档案中记录，暂不立条目，待能播放时补。另有 12 条已摘录但本批未立条目（图片材质、电影感、触感、5种导航、命令面板、脱模板方法论、官网滚动、加载7种、弹窗7种、术语库、设置页以外的 Vibe 集数等），要点已在本节档案中保留，可后续提升为条目。作者称其 Skills 已开源在 GitHub 仓库 `spt-ui-interaction-skills`（文案说法，本次未核到确切网址），若后续取得仓库原文，可据原文升级这些条目。

### 本批新增待验证条目（20 条）


#### SpicyTater：下拉组件 8 种选型 (`spt-dropdown-8`)

```json
{
  "id": "spt-dropdown-8",
  "title": "SpicyTater：下拉组件 8 种选型",
  "category": "细节优化",
  "styles": [
    "下拉",
    "组件选型",
    "章节摘录"
  ],
  "scenario": "做下拉选择，不知道用哪种下拉形态时",
  "prompt": "Pick the dropdown form by the job: plain Dropdown for choosing one from a few fixed options; grouped dropdown (bus/group headers) when options are many; Typeahead searchable dropdown filtering as you type; Split action button — main area runs the primary action, the drop zone offers related actions; Date range picker via calendar for start/end; Cascade select for parent-child options, choosing a level expands the next; Tag Picker for multi-select, keeping chosen tags visible; Mega Menu for content-rich sites with many sections in multiple columns. State the option count, grouping, search and action model when asking an AI to build one.",
  "prompt_zh": "SpicyTater 第7集（1057赞/1239收藏）：Dropdown/分组下拉/Typeahead/拆分按钮/日期范围/级连/Tag Picker/Mega Menu 8 种下拉，按数量、分组、搜索、操作选型。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7680742171204439296"
}
```

#### SpicyTater：浮层 6 种选型与 3 个坑 (`spt-overlay-six`)

```json
{
  "id": "spt-overlay-six",
  "title": "SpicyTater：浮层 6 种选型与 3 个坑",
  "category": "细节优化",
  "styles": [
    "浮层",
    "弹窗选型",
    "章节摘录"
  ],
  "scenario": "纠结用弹窗、抽屉还是新页面时",
  "prompt": "Choose overlay components by weight: Tooltip — quietest, small text on hover, gone on leave; Toast — fleeting, for operation results; Alert — persistent, for important notices; Modal — for important decisions; plus Popconfirm for inline confirmation and Drawer for side content. Avoid three traps: don't close modals on backdrop click when there's unsaved input (add draft autosave instead); don't demand confirmation for deletable-and-undoable actions; write the action's result directly on the button. Long forms don't belong squeezed inside a small modal — use a drawer or a full page.",
  "prompt_zh": "SpicyTater 第28集（848赞/843收藏）：Tooltip/Toast/Alert/Modal/Popconfirm/Drawer 选型 + 三坑（蒙层误关配草稿保存、可撤销别弹窗确认、按钮直写结果）。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7699199951179418907"
}
```

#### SpicyTater：交互质感 8 指令 (`spt-app-texture-8`)

```json
{
  "id": "spt-app-texture-8",
  "title": "SpicyTater：交互质感 8 指令",
  "category": "细节优化",
  "styles": [
    "动效",
    "质感",
    "章节摘录"
  ],
  "scenario": "想要 App 交互有物理质感、遵循统一运动规则时（动效类）",
  "prompt": "Give interface motion one consistent physics: magnetic snap — resistance while approaching a target, acceleration inside the snap range, elastic settle at the end; liquid deformation — dragged cards stretch at edges and recover with a rebound on release; 3D parallax — foreground moves most, midground less, background slightly; center focus — items near screen center scale up, leaving items shrink or fade in weight; liquid tab — the selected background stretches horizontally, contracts past the midpoint, then a slight rebound; image expansion — from thumbnail to fullscreen with continuous direction and position; gesture-driven transitions whose progress follows the finger and completes past a threshold; collision push — elements have different motion weights, pushing and rebounding on contact.",
  "prompt_zh": "SpicyTater 第10集（511赞）：磁吸/液态形变/3D视差/中心聚焦/液态tab/图片展开/手势转场/碰撞推挤 8 种质感指令，核心是全场遵循同一套运动规则。动效类，验证需 GIF。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7682010730085862696"
}
```

#### SpicyTater：App 高级交互 7 指令 (`spt-app-gestures-7`)

```json
{
  "id": "spt-app-gestures-7",
  "title": "SpicyTater：App 高级交互 7 指令",
  "category": "细节优化",
  "styles": [
    "手势",
    "App交互",
    "章节摘录"
  ],
  "scenario": "做移动端手势交互、总觉得不跟手时",
  "prompt": "Implement these mobile gesture rules: edge-swipe back — drag from the screen edge pulls the previous page with the finger, release decides by distance, velocity and direction; press-and-slide-off cancel — pressing sinks the button, sliding out weakens the press state, releasing outside cancels the tap; partial text transition — when filters change, only the changed text transitions, unchanged text stays put; gesture direction lock — decide the direction at gesture start and never flip mid-gesture; interruptible animation takeover — a gesture can seize a running animation and continue from the element's current position; landing preview — while dragging a card horizontally, preview its predicted landing spot and land exactly there; boundary damping — pulling past the top keeps moving with increasing resistance, then springs back on release.",
  "prompt_zh": "SpicyTater 第11集（1225赞）：跟手返回/滑出取消/文字局部过渡/方向锁定/动画中途接管/落点预览/边界阻尼 7 条高级交互指令。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7682681851068026152"
}
```

#### SpicyTater：展开动画 6 种 (`spt-expand-animations`)

```json
{
  "id": "spt-expand-animations",
  "title": "SpicyTater：展开动画 6 种",
  "category": "细节优化",
  "styles": [
    "动效",
    "展开",
    "章节摘录"
  ],
  "scenario": "小组件需要展开成大内容时（动效类）",
  "prompt": "Use these expansion patterns: dot-to-capsule — a circle expands into a capsule carrying a status or short message; capsule-to-card — a compact capsule expands into a full info card with more content and actions; compact-to-panel — the same feature appears compact first and expands into a full control panel when needed; radius morph — changing corner radius morphs one form smoothly into another; size morph — animate width and height so a small widget becomes a larger module; content reflow — after expanding, inner content rearranges, and collapsing retraces the same path back to the small entry. Always specify start state, end state, which properties change, and how it collapses back.",
  "prompt_zh": "SpicyTater 第6集（308赞）：圆点变胶囊/胶囊变信息卡/紧凑态展开/圆角形态过渡/尺寸变形/内容重排，描述时讲清起止状态、变化属性、收回方式。动效类，验证需 GIF。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7680037853694381327"
}
```

#### SpicyTater：像产品不像作业的六步 (`spt-product-not-homework`)

```json
{
  "id": "spt-product-not-homework",
  "title": "SpicyTater：像产品不像作业的六步",
  "category": "细节优化",
  "styles": [
    "方法论",
    "产品级",
    "章节摘录"
  ],
  "scenario": "AI 做的页面总像模板作业、想做到产品级时",
  "prompt": "Take an AI-built page from homework to product in six steps: 1) design system first — unify fonts, colors, radii, spacing and component styles; 2) page structure — clarify navigation, content hierarchy and layouts across screen sizes; 3) interaction flows — define what happens on every click plus empty, loading, success and failure states; 4) concept image to confirm direction and visual focus; 5) real functionality — buttons, forms and data flows actually work; 6) detail pass — assets, responsive layout and interaction feedback.",
  "prompt_zh": "SpicyTater 第14集（271赞，12分钟）：先定规范→搭结构→补交互流程（含空/加载/成功/失败态）→概念图定方向→落地真实功能→打磨细节。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7687151464640220456"
}
```

#### SpicyTater：导航组件 7 种选型 (`spt-nav-7`)

```json
{
  "id": "spt-nav-7",
  "title": "SpicyTater：导航组件 7 种选型",
  "category": "细节优化",
  "styles": [
    "导航",
    "组件选型",
    "章节摘录"
  ],
  "scenario": "给页面选导航组件时",
  "prompt": "Choose navigation components precisely: Tabs for switching parallel content within one page; Segmented Control for fast switching between 2-3 views (fewer options, tighter layout); Breadcrumb for deep hierarchies, showing current position and quick return; Pagination for browsing large content by page; Stepper for process progress, showing done and remaining steps; Sidebar for feature-rich backends/desktops, fixed main entries with the current page highlighted; Bottom Navigation for mobile, 3-5 frequent entries fixed at the bottom. When asking an AI, name the component, its placement, what it switches and what gets highlighted.",
  "prompt_zh": "SpicyTater 第3集（227赞）：Tabs/Segment Control/Breadcrumb/Pagination/Stepper/Sidebar/Bottom Navigation 7 种导航的适用与描述要点。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7678886080376098086"
}
```

#### SpicyTater：拖拽动效 6 种 (`spt-drag-6`)

```json
{
  "id": "spt-drag-6",
  "title": "SpicyTater：拖拽动效 6 种",
  "category": "细节优化",
  "styles": [
    "拖拽",
    "动效",
    "章节摘录"
  ],
  "scenario": "界面需要拖拽类交互时",
  "prompt": "Implement the right drag pattern for the job: drag-and-drop — drag an object to a target zone, release to place or move; drag-to-sort — drag a list item while others auto-shift, save the new order on release; slider drag — drag a thumb to adjust a value, progress or option; drag-to-resize — drag an edge or corner to change width/height; drag-to-select — drag on empty space to draw a selection box over multiple objects; drag-to-upload — drag files into a marked zone with clear feedback. Each needs its drag direction, draggable area, target and release feedback spelled out.",
  "prompt_zh": "SpicyTater 第5集（192赞）：拖放/拖拽排序/滑块拖动/拖拽调整大小/拖拽框选/拖拽上传 6 种，描述须含方向、区域、目标与松手反馈。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7679648378807979305"
}
```

#### SpicyTater：空间卡片编排 6 种 (`spt-card-arrangements`)

```json
{
  "id": "spt-card-arrangements",
  "title": "SpicyTater：空间卡片编排 6 种",
  "category": "细节优化",
  "styles": [
    "卡片编排",
    "展示",
    "章节摘录"
  ],
  "scenario": "作品集/相册想要非常规的卡片展示方式时",
  "prompt": "Arrange showcase cards spatially: fan spread — cards fan around a pivot like playing cards, clicking one lifts it (covers, collections); depth stack — cards offset along depth for browsing one by one; cylinder ring — cards wrap a cylinder, drag to rotate (portfolios, albums, projects); sphere layout — cards distributed on a sphere for exploring photos/inspiration; spiral layout — cards along a spiral path (project stages, timelines); wave matrix — a tidy grid where neighbours offset in rhythm (photo walls, overviews). When asking an AI, specify the arrangement, the browsing method, how selection is shown and where cards return on close.",
  "prompt_zh": "SpicyTater 第15集（171赞）：扇形展开/纵深叠排/圆柱环绕/球面排布/螺旋排布/波浪矩阵 6 种空间卡片编排及适用场景。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7687510825015315712"
}
```

#### SpicyTater：点击区域与反馈五查 (`spt-tap-feedback`)

```json
{
  "id": "spt-tap-feedback",
  "title": "SpicyTater：点击区域与反馈五查",
  "category": "细节优化",
  "styles": [
    "点击热区",
    "反馈",
    "章节摘录"
  ],
  "scenario": "界面精致但点不动、点不准时",
  "prompt": "Audit tap usability: hit area — icons may be small but buttons must not shrink with them; size touch targets in CSS pixels adjusted per platform; hot-zone conflicts — fix overlaps by adjusting spacing and layout; distinguish tap from drag so gestures never misfire; feedback must be explicit — pressed state change, submitting state, and failure notice. When briefing an AI, always check: hit areas, hot-zone conflicts, links, tap-vs-drag distinction, and feedback states.",
  "prompt_zh": "SpicyTater 第32集：点击范围（图标小按钮不能小）/热区冲突/区分点击与拖动/点击反馈明确（按下变化、提交状态、失败提示）五查。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7705257186435403058"
}
```

#### SpicyTater：卡片/列表/表格按任务选型 (`spt-layout-by-task`)

```json
{
  "id": "spt-layout-by-task",
  "title": "SpicyTater：卡片/列表/表格按任务选型",
  "category": "细节优化",
  "styles": [
    "布局选型",
    "数据展示",
    "章节摘录"
  ],
  "scenario": "挑图片、找文件、比数据不知道用卡片还是列表时",
  "prompt": "Match data layout to the task: cards for browsing visual items (photos, furniture) — big image first, name in one line; lists for finding a known file — small thumbnail aside, full name expanded; tables for comparing data — show name, dimensions, format with the same data aligned in columns. When switching layouts, preserve the search conditions and selection state so the user never has to redo their work.",
  "prompt_zh": "SpicyTater 第29集：卡片适合展示、列表适合查找、表格适合比数据；切换布局保留搜索条件与勾选状态。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7699718828174937379"
}
```

#### SpicyTater：选择器与菜单别混用 (`spt-picker-menu`)

```json
{
  "id": "spt-picker-menu",
  "title": "SpicyTater：选择器与菜单别混用",
  "category": "细节优化",
  "styles": [
    "下拉",
    "选型",
    "章节摘录"
  ],
  "scenario": "跟 AI 说做个下拉框总不好用时",
  "prompt": "Distinguish pickers from menus: a picker selects a value, a menu issues an action. Few options can be shown directly; when they don't fit, use a picker; two options are not automatically a toggle switch. Many options need grouping and a scrollable list that never overflows the screen. Familiar values can be typed directly; when space is tight, flip the opening direction. When briefing an AI, state: what is being chosen, what happens after choosing, and where the result stays. A music app's 'pick a song and keep browsing' is not the same as 'choose an action and dismiss'.",
  "prompt_zh": "SpicyTater 第31集：选择器用于选择、菜单用于操作；选项少直展、多则分组滚动；明确选什么、选完做什么、结果留在哪。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7701961806482279715"
}
```

#### SpicyTater：底部浮层 5 种区分 (`spt-bottom-layers`)

```json
{
  "id": "spt-bottom-layers",
  "title": "SpicyTater：底部浮层 5 种区分",
  "category": "移动端App",
  "styles": [
    "底部浮层",
    "组件选型",
    "章节摘录"
  ],
  "scenario": "移动端底部弹出的东西分不清该用哪种时",
  "prompt": "Tell bottom layers apart: Action Sheet — bottom action panel, dismisses right after choosing; Bottom Sheet — expandable sheet that stays where released, its inner content can scroll (e.g. keep browsing songs); Snack Bar — bottom notice whose height follows content and screen, never full-screen by default; Tour — guided walkthrough that skips steps the user already knows; Lightbox — image viewer for detail, without leaving the page; plus inline validation — show the error where it happened.",
  "prompt_zh": "SpicyTater 第30集：Action Sheet/Bottom Sheet/Snack Bar/Tour/Lightbox 五种底部浮层的区别与行内验错。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7701274323436227880"
}
```

#### SpicyTater：多语言按钮防挤爆 (`spt-i18n-overflow`)

```json
{
  "id": "spt-i18n-overflow",
  "title": "SpicyTater：多语言按钮防挤爆",
  "category": "细节优化",
  "styles": [
    "国际化",
    "响应式",
    "文案摘录"
  ],
  "scenario": "界面切换语言后按钮被长译文挤爆时",
  "prompt": "Design buttons for long translations: never shrink the font to force-fit long text; let buttons grow with content, allow the action bar to wrap, or switch to full-width taller buttons; then verify with real translations, narrow windows and larger font sizes, checking for clipping, collisions and horizontal overflow.",
  "prompt_zh": "SpicyTater 第35集：长译文别缩字硬塞；让按钮增长、操作栏换行或全宽增高；用真实译文+窄窗口+大字号查裁切/碰撞/横向溢出。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7707974421738278187"
}
```

#### SpicyTater：圆角看整体轮廓 (`spt-radius-contour`)

```json
{
  "id": "spt-radius-contour",
  "title": "SpicyTater：圆角看整体轮廓",
  "category": "细节优化",
  "styles": [
    "圆角",
    "轮廓",
    "文案摘录"
  ],
  "scenario": "圆角越调越大还是不像设计稿时",
  "prompt": "Fix corner radius as a whole contour, not a number: stop only increasing the radius; lock the element's size and layout first, then compare the corner transition curve; make image clipping, strokes and shadows all follow the same contour; finally re-check at normal size and in narrow cards for show-through gaps and squeezed text.",
  "prompt_zh": "SpicyTater 第34集：别只改半径；锁尺寸布局、比转弯过渡、让裁切/描边/阴影沿用同一轮廓、回正常与窄卡片查露底挤字。与已验证的同心圆角互补。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7707970051038645546"
}
```

#### SpicyTater：聊天页滚动位置锚定 (`spt-chat-scroll-anchor`)

```json
{
  "id": "spt-chat-scroll-anchor",
  "title": "SpicyTater：聊天页滚动位置锚定",
  "category": "AI产品",
  "styles": [
    "聊天界面",
    "滚动",
    "文案摘录"
  ],
  "scenario": "聊天页新消息一来就把用户拽走时",
  "prompt": "Anchor chat scrolling to the reader: new messages may keep streaming in, but never decide for the user where they are reading; when the user scrolls up, pause auto-follow; resume following when they return to the bottom; when loading history above, keep the currently read message exactly in place.",
  "prompt_zh": "SpicyTater 第36集（2026-11-17 当天新作）：上翻暂停跟随、回到底部恢复、加载历史保住当前消息位置。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7707976118627798312"
}
```

#### SpicyTater：图片交互 7 种 (`spt-image-interactions-7`)

```json
{
  "id": "spt-image-interactions-7",
  "title": "SpicyTater：图片交互 7 种",
  "category": "细节优化",
  "styles": [
    "图片交互",
    "动效",
    "章节摘录"
  ],
  "scenario": "给图片展示加高级交互时（多为动效类）",
  "prompt": "Add advanced image interactions: before-after slider — drag a divider to change the revealed range; mask reveal — pointer or finger movement uncovers the image; pixel transition — pixel blocks cover the frame then dissolve to reveal the next image; ripple distortion — ripples follow the pointer and decay after it stops; sticker peel — the image peels from a corner like a sticker, revealing content beneath; image trail — images spawn along the pointer path and shrink/fade after a pause; glare hover — a highlight follows the pointer across the card.",
  "prompt_zh": "SpicyTater 图片交互篇：前后对比滑块/遮罩揭示/像素转场/水波扭曲/贴纸揭起/图片拖尾/悬停反光 7 种。动效类，验证需 GIF。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7682679805443149108"
}
```

#### SpicyTater：无限画布 5 指令 (`spt-infinite-canvas`)

```json
{
  "id": "spt-infinite-canvas",
  "title": "SpicyTater：无限画布 5 指令",
  "category": "细节优化",
  "styles": [
    "无限画布",
    "协作工具",
    "章节摘录"
  ],
  "scenario": "做白板/无限画布类产品时",
  "prompt": "Build infinite-canvas interactions: pan & zoom — zoom around the pointer position, drag empty space to pan, cards keep relative positions; multi-selection & grouping — rubber-band select and group, moving a group keeps internal distances; connector binding — connectors bind to cards and anchor points, paths update while dragging, support reconnect and delete; auto layout — arrange by content type while preserving connectors and groups, with undo; minimap navigation — minimap shows content distribution and the current viewport, click to jump, drag the viewport box.",
  "prompt_zh": "SpicyTater 第13集：缩放中心/框选成组/连线绑定/自动布局/小地图导航 5 条无限画布指令。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-17T23:11:51+08:00",
  "source": "SpicyTater 抖音（2026-11-17 收集；视频未能播放，要点据页面文案与抖音章节要点摘录，非逐字原文）",
  "source_video": "https://www.douyin.com/video/7684165291919543586"
}
```

## 2026-11-18 · 公开渠道收集（StyleKit / ByteMint / Superdesign / YouTube 车机教程）

来源核对：新拟态提示词见 Vibe Coder《Web Design Guide》1.2 节（搜索结果原文）；孟菲斯/包豪斯风格定义见 StyleKit 151 风格库与 ByteMint UI 提示词库（搜索结果原文），提示词按风格定义原创改写；交易邮件提示词见 Superdesign《UI Design Prompts》(2026) 第 8 节（已打开页面核对原文）；车机提示词据 YouTube《How to Vibe Code a Car Dashboard with Claude》简介中的计划提示词摘要改写。以上 5 条均为库里没有的风格/场景（新拟态、孟菲斯、包豪斯、车机 UI、邮件模板），只进待验证区。

#### 新拟态音乐播放器 (`style-neumorphism-player`)

```json
{
  "id": "style-neumorphism-player",
  "title": "新拟态音乐播放器",
  "category": "内容社交",
  "styles": [
    "新拟态",
    "柔和立体",
    "音乐播放器"
  ],
  "scenario": "音乐播放器/控制面板想要柔和立体触感时",
  "prompt": "Create a neumorphism music player dashboard on a #e0e5ec background. Build raised circular play/pause buttons using dual box-shadows: box-shadow: 6px 6px 12px #b8bec7, -6px -6px 12px #ffffff. Add pressed (active) state with inset shadows: inset 4px 4px 8px #b8bec7, inset -4px -4px 8px #ffffff. Include a volume slider and a track progress bar in the same neumorphic style; album art sits in a soft recessed well, track title and artist in dark gray. Keep every element the same #e0e5ec tone so depth comes only from shadows, and keep text contrast readable.",
  "prompt_zh": "新拟态音乐播放器：#e0e5ec 同色底、双向阴影做出凸起与按压、圆形播放键+音量滑杆+进度条，深度只靠阴影，文字对比度要可读。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-18T08:20:00+08:00",
  "source": "Vibe Coder《Web Design Guide》1.2 新拟态节（搜索结果原文核对，2026-11-18）"
}
```

#### 孟菲斯撞色落地页 (`landing-memphis`)

```json
{
  "id": "landing-memphis",
  "title": "孟菲斯撞色落地页",
  "category": "落地页官网",
  "styles": [
    "孟菲斯",
    "撞色",
    "几何"
  ],
  "scenario": "创意/潮流品牌落地页想要 80 年代孟菲斯活力时",
  "prompt": "Design a landing page in Memphis style, the 80s Italian design movement: bold geometric shapes (circles, triangles, squiggles, grids), vivid contrasting colors (hot pink, yellow, teal, black), irregular playful patterns that break the grid, thick black outlines, oversized geometric headline type. Hero with a big geometric composition, feature cards as tilted color blocks with hard shadows, playful scattered shapes across sections. Keep the copy short and the layout energetic but readable; one clear primary CTA.",
  "prompt_zh": "孟菲斯风落地页：大胆几何图形+高饱和撞色+不规则图案+粗黑描边，活力十足但文案要短、主按钮唯一。",
  "tools": [
    "v0",
    "Lovable",
    "Framer"
  ],
  "group": {
    "id": "landing-styles",
    "name": "落地页官网 · 风格组"
  },
  "variant_label": "孟菲斯撞色几何",
  "added_at": "2026-11-18T08:20:00+08:00",
  "source": "StyleKit 151 风格库 + ByteMint UI 提示词库孟菲斯条目（搜索结果原文核对；提示词按风格定义原创改写，同类收集，2026-11-18）"
}
```

#### 包豪斯几何官网 (`landing-bauhaus`)

```json
{
  "id": "landing-bauhaus",
  "title": "包豪斯几何官网",
  "category": "落地页官网",
  "styles": [
    "包豪斯",
    "几何",
    "现代主义"
  ],
  "scenario": "设计/建筑/文化机构官网想要包豪斯现代主义时",
  "prompt": "Design a website in Bauhaus style: functionalist modernism built only from circles, squares and triangles, thick black borders, hard offset shadows, and pure Bauhaus primaries (red, blue, yellow) plus black and off-white. Asymmetric architectural layout, oversized geometric headline, grid-based sections, no gradients, no rounded corners, no decoration beyond geometry. Form follows function — every shape earns its place.",
  "prompt_zh": "包豪斯风官网：只用圆/方/三角+粗黑边+硬偏移阴影+红蓝黄三原色，非对称建筑感布局，无渐变无圆角。",
  "tools": [
    "v0",
    "Framer",
    "Cursor"
  ],
  "group": {
    "id": "landing-styles",
    "name": "落地页官网 · 风格组"
  },
  "variant_label": "包豪斯几何原色",
  "added_at": "2026-11-18T08:20:00+08:00",
  "source": "StyleKit 151 风格库 + ByteMint UI 提示词库包豪斯条目（搜索结果原文核对；提示词按风格定义原创改写，同类收集，2026-11-18）"
}
```

#### 车机中控屏：特斯拉风 (`car-infotainment-tesla`)

```json
{
  "id": "car-infotainment-tesla",
  "title": "车机中控屏：特斯拉风",
  "category": "车机出行",
  "styles": [
    "车机",
    "深色",
    "信息娱乐"
  ],
  "scenario": "车机/中控大屏 UI 设计时",
  "prompt": "Design a Tesla-style car infotainment screen, 1280x720 landscape touchscreen, plain HTML/CSS/JS, no photos: left third shows a top-down car in inline SVG, gear selector P R N D, large speed readout, battery percentage and range; right panel shows a stylised city map with a blue route line, next-turn card and ETA; bottom dock holds driver temperature, music controls, fan speed and seat controls. Colors: base #0B0D10, glass panels #15181D, borders #262B33, accent cyan #2FD3FF, text #E8ECF1. Big touch targets, glanceable while driving, no small text.",
  "prompt_zh": "特斯拉风车机中控：1280×720 横屏、左车况+中地图+下快捷坞，深色玻璃面板+青色强调色，驾驶时一眼可读。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-18T08:20:00+08:00",
  "source": "YouTube《How to Vibe Code a Car Dashboard with Claude》（据视频简介的计划提示词摘要改写，同类收集，2026-11-18）"
}
```

#### 交易邮件模板：欢迎/验证 (`email-transactional`)

```json
{
  "id": "email-transactional",
  "title": "交易邮件模板：欢迎/验证",
  "category": "邮件模板",
  "styles": [
    "邮件",
    "交易邮件",
    "极简"
  ],
  "scenario": "欢迎/验证类交易邮件模板设计时",
  "prompt": "Design a welcome / email-verification transactional email. Single-column layout, max 600px wide, works in dark and light mail clients. Structure: small logo at top, a clear headline, one short paragraph of context, one prominent primary button (the single action), a plain-text fallback link under it, and a simple footer (company, address, unsubscribe). Visual system: minimal, high-contrast, one brand color on the button only, system fonts, generous padding. Tone: warm and human, one sentence of personality. Avoid image-only emails, multiple competing CTAs, and tiny tap targets.",
  "prompt_zh": "交易邮件（欢迎/验证）：单栏 600px、一个主按钮+纯文本备用链接、系统字体、品牌色只用在按钮上，深浅邮件客户端都可用。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-18T08:20:00+08:00",
  "source": "Superdesign《UI Design Prompts: A Copy-Paste Library for Real Interfaces (2026)》第 8 节（已打开页面核对原文，括号占位按通用版整理，2026-11-18）"
}
```

## 2026-11-18 · 公开渠道收集（第二轮：旅行/引导/智能家居/仪表盘可读性/播客）

来源：HitPaw《GPT Image 2 Prompts for UI Design》旅行与智能家居节、Lovable UI prompts（新手引导流程、空/加载状态）、Medium《Dashboard UI Design: 12 Real App Examples》（仪表盘可读性九项检查）、Design Lounge《Slow Archive podcast player》（章节波形播客播放器）、UXCharan《216 AI Prompts for UX/UI Designers》（新手引导文案）。以上均为搜索结果原文核对；提示词按主题原创改写，标注「同类收集，非原作摘录」，不冒充原作逐字摘录。已与正式库 29 条 + 待验证区去重：空/加载状态与正式库 detail-states-complete 同主题已跳过，深色渐变落地页与 landing-ai-product（深色科技渐变 variant）同风格已跳过。

### 旅行预订 App：沉浸式搜索+预订 (`mobile-travel-booking`)

```json
{
  "id": "mobile-travel-booking",
  "title": "旅行预订 App：沉浸式搜索+预订",
  "category": "移动端App",
  "styles": [
    "旅行预订",
    "沉浸式",
    "图片主导"
  ],
  "scenario": "做机票/酒店预订 App，想要图片主导的沉浸式预订流程时",
  "prompt": "Design a mobile travel booking app: home opens with a large immersive destination photo and a clean search bar (destination, dates, travellers) overlaid at the bottom; below, horizontally scrolling destination cards with price-from labels and a 'Trending now' row. Tapping a destination opens a detail screen with a photo gallery, a date picker, guest stepper and a sticky bottom bar showing total price and a single 'Book now' button. Flight results show a glowing route line on a small map, departure/arrival times and one clear cheapest-fastest toggle. Use elegant serif headlines with clean sans-serif body text, warm neutral palette with one terracotta accent, generous whitespace, 16px corner radius on cards. Every step must answer in one tap — no dead-end screens.",
  "prompt_zh": "旅行预订 App：大图沉浸式首页+底部搜索条、目的地横滑卡片、详情页含日期选择与常驻总价预订栏，航班结果带路线图与最便宜/最快切换，衬线标题+陶土强调色。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-18T09:30:00+08:00",
  "source": "HitPaw《GPT Image 2 Prompts for UI Design》第 8 节旅行预订 + aiarty 旅行预订条目（搜索结果原文核对；提示词按主题原创改写，同类收集，非原作摘录，2026-11-18）"
}
```

## 2026-11-19 · 公开渠道收集（Visualizee.ai 游戏 UI / Carat 简历设计）

来源：Visualizee.ai《Game UI Design with AI: Interface Mockups Fast》（HUD、主菜单、背包三节）、Carat《Resume Design Prompts》（极简双栏、信息图简历两条）。以上均为已打开页面核对原文，提示词为原文摘录；库里此前没有游戏 UI 与简历/文档类条目，已与正式库 37 条 + 待验证区去重，无重复。

### 科幻射击游戏 HUD：血条/弹药/小地图 (`game-hud-scifi`)

```json
{
  "id": "game-hud-scifi",
  "title": "科幻射击游戏 HUD：血条/弹药/小地图",
  "category": "游戏娱乐",
  "styles": [
    "游戏UI",
    "HUD",
    "科幻",
    "全息"
  ],
  "scenario": "做科幻射击游戏，需要血条、弹药、小地图一目了然的全息 HUD 时",
  "prompt": "Design a sci-fi shooter HUD. Include health bar in top-left, ammunition counter in bottom-right, minimap radar in top-right corner. Holographic blue style with glowing edges, transparent panels, futuristic sans-serif typography. Clean and readable against dark backgrounds.",
  "prompt_zh": "科幻射击 HUD：左上血条、右下弹药、右上雷达小地图，全息蓝发光边缘+透明面板，未来感无衬线字体，深色背景上清晰可读。",
  "tools": [
    "即梦",
    "Midjourney",
    "v0"
  ],
  "source": "Visualizee.ai《Game UI Design with AI: Interface Mockups Fast》HUD 一节（已打开页面核对原文，提示词为原文摘录，2026-11-19）",
  "added_at": "2026-11-19T08:10:00+08:00"
}
```

### 休闲农场模拟游戏主菜单 (`game-main-menu-cozy`)

```json
{
  "id": "game-main-menu-cozy",
  "title": "休闲农场模拟游戏主菜单",
  "category": "游戏娱乐",
  "styles": [
    "游戏UI",
    "主菜单",
    "休闲",
    "手绘"
  ],
  "scenario": "做休闲模拟经营游戏，需要温暖治愈的主菜单时",
  "prompt": "Create a main menu for a cozy farming simulation game. Centered game logo at top, vertical button stack below: New Game, Continue, Settings, Quit. Soft pastel colors, rounded corners, hand-painted style with watercolor textures. Warm and inviting atmosphere.",
  "prompt_zh": "休闲农场游戏主菜单：顶部居中 Logo，下方竖排新游戏/继续/设置/退出，柔和粉彩+圆角+手绘水彩质感，温暖治愈。",
  "tools": [
    "即梦",
    "Midjourney",
    "v0"
  ],
  "source": "Visualizee.ai《Game UI Design with AI: Interface Mockups Fast》主菜单一节（已打开页面核对原文，提示词为原文摘录，2026-11-19）",
  "added_at": "2026-11-19T08:10:00+08:00"
}
```

### RPG 背包/装备界面：网格物品栏+角色剪影 (`game-inventory-rpg`)

```json
{
  "id": "game-inventory-rpg",
  "title": "RPG 背包/装备界面：网格物品栏+角色剪影",
  "category": "游戏娱乐",
  "styles": [
    "游戏UI",
    "背包",
    "RPG",
    "暗黑奇幻"
  ],
  "scenario": "做 RPG 游戏，需要物品栏+装备栏的背包界面时",
  "prompt": "Design an RPG inventory interface. Grid-based item slots on the left, character equipment panel on the right showing equipped items on a character silhouette. Dark fantasy style with stone textures, metallic borders, subtle glow on magical items. Include tabs for Weapons, Armor, Consumables, Quest Items.",
  "prompt_zh": "RPG 背包界面：左侧网格物品栏、右侧角色剪影装备栏，暗黑奇幻风石材质+金属边框，魔法物品微光，含武器/防具/消耗品/任务物品四个页签。",
  "tools": [
    "即梦",
    "Midjourney",
    "v0"
  ],
  "source": "Visualizee.ai《Game UI Design with AI: Interface Mockups Fast》背包/装备一节（已打开页面核对原文，提示词为原文摘录，2026-11-19）",
  "added_at": "2026-11-19T08:10:00+08:00"
}
```

### 极简双栏简历模板：照片+技能条+时间线 (`doc-resume-minimal`)

```json
{
  "id": "doc-resume-minimal",
  "title": "极简双栏简历模板：照片+技能条+时间线",
  "category": "简历文档",
  "styles": [
    "简历",
    "双栏",
    "极简",
    "模板"
  ],
  "scenario": "做求职简历模板，需要专业干净的双栏 A4 版式时",
  "prompt": "A single A4 resume template design viewed from directly above on a light gray marble surface. Clean two-column layout: left sidebar with circular profile photo placeholder, skill bars, and contact icons; right main area with section headers and timeline entries. Professional navy blue and white color scheme with thin gold accent lines. Modern sans-serif typography placeholder blocks. Crisp flat lay photography with even studio lighting and subtle paper shadow. No readable text, no watermark.",
  "prompt_zh": "极简双栏简历模板：A4 平铺俯拍，左侧圆形照片占位+技能条+联系方式，右侧标题区+时间线条目，藏青白配色+细金线，现代无衬线字体占位块。",
  "tools": [
    "即梦",
    "Midjourney",
    "GPT Image"
  ],
  "source": "Carat《Resume Design Prompts》Minimal Resume Template（已打开页面核对原文，提示词为原文摘录，2026-11-19）",
  "added_at": "2026-11-19T08:10:00+08:00"
}
```

### 信息图风格简历：环形技能图+时间线 (`doc-resume-infographic`)

```json
{
  "id": "doc-resume-infographic",
  "title": "信息图风格简历：环形技能图+时间线",
  "category": "简历文档",
  "styles": [
    "简历",
    "信息图",
    "创意",
    "模板"
  ],
  "scenario": "做创意岗简历，想要信息图风格一页讲清经历与技能时",
  "prompt": "A creative infographic-style resume design on a single A4 page, viewed from above on a concrete desk surface. Visual elements include circular progress charts for skills, timeline graphics for work experience, and icon-based contact section. Modern color palette of teal, charcoal, and soft coral. Clean geometric layout with generous white space. Thin lines connecting sections. Flat lay photography with directional lighting creating soft shadow on one edge. No readable text, no watermark.",
  "prompt_zh": "信息图风格简历：A4 一页，技能环形进度图+经历时间线+图标联系区，青/炭/珊瑚配色，几何布局大留白，细线连接各区。",
  "tools": [
    "即梦",
    "Midjourney",
    "GPT Image"
  ],
  "source": "Carat《Resume Design Prompts》Infographic Resume Design（已打开页面核对原文，提示词为原文摘录，2026-11-19）",
  "added_at": "2026-11-19T08:10:00+08:00"
}
```

## 2026-11-19 · 公开渠道收集（登录页/日历/结账/个人主页）

来源核对：登录页见 Superdesign 登录页提示词库（搜索结果原文：社交登录优先、单密码框、单主按钮、找回链接、具体报错）；日历/日程与个人主页见 Techpresso《30 Claude Prompts That Design UI Screens》对应节（搜索结果原文）；结账见 Techpresso《30 Claude Prompts That Build Checkout Pages》购物车到支付节（搜索结果原文）。以上 4 条均为库里没有的页面类型（登录页、日历、结账、个人主页），只进待验证区；提示词按来源要点原创改写，标注「同类收集，非原作摘录」。

#### 登录页：社交登录优先+单主按钮 (`auth-login-page`)

```json
{
  "id": "auth-login-page",
  "title": "登录页：社交登录优先+单主按钮",
  "category": "SaaS后台",
  "styles": [
    "登录",
    "表单",
    "极简"
  ],
  "scenario": "做登录页、默认模板总把注册和登录混在一起时",
  "prompt": "Design a login page for a SaaS product: sign-in providers first — Google, Apple and GitHub buttons plus a passkey/magic-link option above an 'or with email' divider, so most returning users never type a password. The form: email and one password field with a show-password toggle; no confirm-password field. One primary action: a single solid Log in button; demote sign up to a quiet 'New here? Create an account' link. A 'Forgot password?' link right beside the password field. Specific error copy ('That password is not right. Reset it') and a loading state on the button. Style: neutral base, one accent color on the primary button only, named headline/body typefaces, no purple gradient. A short privacy note under the button and a clear path back to the marketing site.",
  "prompt_zh": "登录页：社交/密钥登录放最前、邮箱+单个密码框带显示切换、一个 Log in 主按钮、注册降级为链接、密码旁放找回链接、写清具体报错与加载态，中性底+单强调色。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T08:18:05+08:00",
  "source": "Superdesign 登录页提示词库（搜索结果原文核对；提示词按模板要点原创改写，同类收集，2026-11-19）"
}
```

#### 日历/日程：月周切换+彩色事件 (`mobile-calendar-schedule`)

```json
{
  "id": "mobile-calendar-schedule",
  "title": "日历/日程：月周切换+彩色事件",
  "category": "移动端App",
  "styles": [
    "日历",
    "日程",
    "移动端"
  ],
  "scenario": "做日历/排班/内容计划界面时",
  "prompt": "Design a calendar/scheduling screen: a top bar with month/week toggle, prev/next arrows, current period label, a Today button and a create-event button; an optional mini-month on the left for navigation; the main grid — a 7-column month grid with weekday headers and date cells, or time-slotted columns for week view. Place color-coded event chips across several cells with one color per event type, one day highlighted as today; use realistic event titles. Today, selected and out-of-month days are visually distinct; event chips keep accessible contrast. Responsive and mobile-first, large tap targets, real form labels and visible focus states.",
  "prompt_zh": "日历/日程屏：顶栏月周切换+前后翻页+今天+新建、左侧可选小月历、主网格 7 列日期格或周视图时间列、事件按类型配色、今天高亮，移动端优先、大点击区。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T08:18:05+08:00",
  "source": "Techpresso《30 Claude Prompts That Design UI Screens》日历/日程节（搜索结果原文核对；提示词按要点原创改写，同类收集，2026-11-19）"
}
```

#### 电商结账：购物车到支付 (`ecom-checkout-flow`)

```json
{
  "id": "ecom-checkout-flow",
  "title": "电商结账：购物车到支付",
  "category": "电商零售",
  "styles": [
    "结账",
    "电商",
    "转化"
  ],
  "scenario": "做电商购物车/结账/订单确认页时",
  "prompt": "Design a cart-to-pay checkout page for an online store: a slim checkout header (Cart current, no marketing nav); line items with image placeholder, name, SKU, unit price, quantity stepper, line total and remove; a summary card with subtotal, shipping options, tax line and estimated total; one primary Continue to pay button; an empty-cart state with a reason to stay and recommendations. Keep money honest: mark any unverified price, tax or shipping figure as to-verify instead of inventing it; no real payment fields on the cart screen. Semantic accessible markup, visible focus, labeled inputs.",
  "prompt_zh": "电商结账：瘦顶栏+商品行（图/名/SKU/单价/数量/小计/删除）+汇总卡（小计/运费/税/预估总价）+继续支付主按钮+空购物车挽留态；金额不确定的标待核对、不编造。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T08:18:05+08:00",
  "source": "Techpresso《30 Claude Prompts That Build Checkout Pages》购物车到支付节（搜索结果原文核对；提示词按要点原创改写，同类收集，2026-11-19）"
}
```

#### 个人主页/账号页：封面+数据+标签页 (`profile-account-page`)

```json
{
  "id": "profile-account-page",
  "title": "个人主页/账号页：封面+数据+标签页",
  "category": "内容社交",
  "styles": [
    "个人主页",
    "账号",
    "社交"
  ],
  "scenario": "做社交/工具类产品的个人主页或账号页时",
  "prompt": "Design a user profile/account screen: a cover/banner band with an overlapping avatar, name, role and one primary action button (Follow / Edit / Message) anchored next to the avatar; a stat row of three to four numbers with labels (posts, followers, following, completion); a tab bar (Overview, Activity, Settings) with one visibly active tab; the default tab shows a bio block, an info card (location, joined date, links) and a recent-activity list. Use realistic sample content; keep the primary action visible on scroll.",
  "prompt_zh": "个人主页：封面横幅+重叠头像+姓名角色+主操作按钮、3–4 项数据行、标签页（概览/动态/设置）、默认页含简介+信息卡+最近动态，主按钮滚动时不丢失。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T08:18:05+08:00",
  "source": "Techpresso《30 Claude Prompts That Design UI Screens》个人主页/账号节（搜索结果原文核对；提示词按要点原创改写，同类收集，2026-11-19）"
}
```

## 2026-11-19 · 公开渠道收集（第二轮：404/通知中心/搜索筛选/学习仪表盘/博客阅读/活动票务）

来源核对：404 错误页见 Medium《Top 10 Easy Prompts for Professional UI Design with designer-skill》（第 10 条，搜索结果原文）与 Liniqo《404 page and error page design》（AI 生成器提示词与插画尺寸要点，搜索结果原文）；通知中心见 design.dev《Toast Notification Stack》提示词模板（四种类型、自动消失进度条）与 JSBits《Design a Notification Center & Toast System》（Toast + 持久通知中心双面结构，搜索结果原文）；搜索筛选见 21st.dev《Filter Menu》与《Search Results》组件说明（分组筛选、可移除 chips、清空全部、键盘导航，搜索结果原文）；学习仪表盘见 danbyers.ai《Build a Learning Dashboard with AI》（顶部四张数据卡+课程/项目进度+深色主题，搜索结果原文）；博客阅读页见同一 Medium 文第 6 条博客主页提示词与 NotVibesCoded UI 提示词库博客类（单栏阅读视图、吸顶目录，搜索结果原文）；活动票务见 Ticko 票务 App 案例研究（发现→详情→选座→结账→票据流程、分区配色选座）与 Showpass 选座地图指南（按票种分区定价、最佳座位推荐，搜索结果原文）。以上 6 条均为库里没有的页面/功能类型，只进待验证区；提示词按来源要点原创改写，标注「同类收集，非原作摘录」，不冒充原作逐字摘录。已与正式库 41 条 + 待验证区 49 条去重：404 与 detail-states-complete（通用空/加载/错误态）不同，是带品牌插画与找回路径的整页；通知中心与 spt-overlay-six（浮层选型）不同，是持久通知列表+Toast 双面系统；学习仪表盘与 saas-dashboard-linear（通用 SaaS 仪表盘）不同，是课程进度/连胜/学习时长场景；博客阅读页与 landing-editorial（杂志风落地页）不同，是长文阅读页而非营销落地页；活动票务与 ecom-checkout-flow（购物车到支付）不同，是选座地图+票种分区流程。

#### 404 错误页：品牌插画+找回路径 (`error-404-page`)

```json
{
  "id": "error-404-page",
  "title": "404 错误页：品牌插画+找回路径",
  "category": "细节优化",
  "styles": [
    "404",
    "错误页",
    "品牌插画"
  ],
  "scenario": "网站出现 404/走丢页面，想把负面体验变成品牌时刻时",
  "prompt": "Design a creative 404 error page for this website that turns a dead end into a brand moment: a friendly one-line apology in plain words ('This page hasn't washed ashore yet' style — say what happened, no error codes as the main text), a small brand-aligned illustration above the message (160-280px on desktop, same illustration style as the site's empty states), a prominent search bar, one clear 'Return to Home' primary button plus links to popular pages, and the site's normal header and footer so it still feels like part of the product. Keep the next step visible without scrolling on a phone, use the site's own colors and typefaces, and return the proper 404 status code.",
  "prompt_zh": "404 错误页：人话道歉+品牌插画（160–280px、与空状态同风格）+醒目搜索框+回首页主按钮与热门页链接，保留站点头尾、手机首屏可见下一步，正确返回 404 状态码。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T09:12:00+08:00",
  "source": "Medium《Top 10 Easy Prompts for Professional UI Design with designer-skill》第 10 条 + Liniqo《404 page and error page design》（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-19）"
}
```

#### 通知中心+Toast 双面系统 (`saas-notification-center`)

```json
{
  "id": "saas-notification-center",
  "title": "通知中心+Toast 双面系统",
  "category": "SaaS后台",
  "styles": [
    "通知",
    "Toast",
    "消息中心"
  ],
  "scenario": "SaaS 产品需要既即时提醒又可回查的通知系统时",
  "prompt": "Build a notification system as two surfaces sharing one data source: (1) ephemeral toasts — stacked vertically top-right with 10px gaps, four types (success, error, warning, info) each with its own accent color, icon, title and message; a 2px auto-dismiss progress bar at the bottom of each toast shrinking from 100% to 0% over its duration, hover pauses the countdown, errors never auto-dismiss, each toast has a close button and a simple show API. (2) a persistent notification center — a panel listing every event with read/unread state, actor avatar, relative time, unread count badge, mark-read and mark-all-read actions, and infinite scroll. Keep the visual language consistent across both surfaces and announce new toasts to screen readers without stealing focus.",
  "prompt_zh": "通知双面系统：右上堆叠 Toast（四种类型各有强调色、2px 倒计时进度条、悬停暂停、错误不自动消失）+ 持久通知中心（已读/未读态、未读角标、一键已读、无限滚动），两面共用同一数据源。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T09:12:00+08:00",
  "source": "design.dev《Toast Notification Stack》提示词模板 + JSBits《Design a Notification Center & Toast System》（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-19）"
}
```

#### 搜索结果页：筛选侧栏+已选 chips (`search-results-filters`)

```json
{
  "id": "search-results-filters",
  "title": "搜索结果页：筛选侧栏+已选 chips",
  "category": "SaaS后台",
  "styles": [
    "搜索",
    "筛选",
    "列表"
  ],
  "scenario": "做内容/商品/文档搜索结果页，需要侧栏筛选时",
  "prompt": "Design a search results page with a filter sidebar: a search bar at the top with the query and result count ('128 results for \"…\"'); a left filter sidebar with collapsible checkbox groups (category, date, type, status), each group showing counts; active filters shown as removable chips above the results with a 'Clear all' action; results as a clean list (title, snippet with the matching text in bold, source and date) or an image grid toggle; a sort control (relevance/newest) and pagination or infinite scroll. On mobile the sidebar collapses into a filter button opening a bottom sheet. Full keyboard navigation, visible focus, and never let filters push results below the fold on desktop.",
  "prompt_zh": "搜索结果页：顶部搜索框+结果数、左侧可折叠复选框筛选分组（带数量）、已选条件以 chips 显示可逐个移除+清空全部、结果列表关键词加粗或图片网格切换、排序与分页，移动端筛选项收进底部浮层。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T09:12:00+08:00",
  "source": "21st.dev《Filter Menu》与《Search Results》组件说明（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-19）"
}
```

#### 在线学习仪表盘：进度+连胜+学习时长 (`edu-learning-dashboard`)

```json
{
  "id": "edu-learning-dashboard",
  "title": "在线学习仪表盘：进度+连胜+学习时长",
  "category": "在线教育",
  "styles": [
    "学习仪表盘",
    "进度",
    "深色"
  ],
  "scenario": "做在线课程/学习平台的个人学习进度仪表盘时",
  "prompt": "Build a learning progress dashboard: a header with the title 'Learning Dashboard' and today's date; a stats row of 4 cards at the top — total lessons completed (out of 24), total projects completed (out of 11), current streak in days, and total study hours — each card with a large number, a label and a small icon; below, two side-by-side sections: on the left a lesson list with animated progress bars and completion checkmarks, on the right weekly progress and study-hours charts plus a streak counter that tracks consecutive days of activity. Use a dark theme with clean modern styling and clear visual hierarchy, progress bars animate on load, and keep the layout scannable at a glance.",
  "prompt_zh": "学习仪表盘：顶栏标题+今日日期、四张数据卡（已完成课时/项目/连续天数/学习时长）、左侧课程列表带动画进度条、右侧周进度与学时图表+连胜计数，深色主题、层级清晰、一眼可读。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T09:12:00+08:00",
  "source": "danbyers.ai《Build a Learning Dashboard with AI》（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-19）"
}
```

#### 博客文章阅读页：单栏+吸顶目录 (`content-blog-reading`)

```json
{
  "id": "content-blog-reading",
  "title": "博客文章阅读页：单栏+吸顶目录",
  "category": "内容社交",
  "styles": [
    "博客",
    "阅读页",
    "长文"
  ],
  "scenario": "做博客/长文内容站，需要舒服的文章阅读页时",
  "prompt": "Design a blog article reading page as a clean single-column reading view: a comfortable measure (around 65-75 characters per line), generous line spacing, warm serif headlines with clean sans-serif body text; a sticky table-of-contents sidebar that highlights the section currently in view as the reader scrolls; a reading-progress bar at the top, author bio block with avatar and follow button, estimated reading time and publish date under the title; at the end, share actions and a 'next article' card. Above the article, a full-width featured-article hero for the latest post, followed by a grid of recent posts with thumbnails, titles and excerpts. Editorial layout, strong spacing, no clutter around the text — reading is the product.",
  "prompt_zh": "博客阅读页：单栏舒适行宽行距、衬线标题+无衬线正文、吸顶目录随滚动高亮当前节、顶部阅读进度条、作者简介与预计阅读时长，文首通栏精选文章+近期文章网格，阅读本身就是产品。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T09:12:00+08:00",
  "source": "Medium《Top 10 Easy Prompts for Professional UI Design with designer-skill》第 6 条博客主页 + NotVibesCoded UI 提示词库博客类（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-19）"
}
```

#### 活动票务：分区选座+订单汇总 (`event-ticket-seat-picker`)

```json
{
  "id": "event-ticket-seat-picker",
  "title": "活动票务：分区选座+订单汇总",
  "category": "电商零售",
  "styles": [
    "票务",
    "选座",
    "活动"
  ],
  "scenario": "做演唱会/演出/赛事票务 App，需要选座购票流程时",
  "prompt": "Design a mobile event ticketing flow in five steps: 1) Discover — event list with poster, date, venue and starting price; 2) Event detail — one screen with date, venue map, short description, and the starting price with a pinned 'Pick a seat' button at the bottom; 3) Pick a seat — a venue seat map with color-coded zones (one color per ticket type, matching the zone list), quantity steppers beside each zone, best-available seat suggestions ranked and shown as a short list, accessible and limited-view seats clearly marked; 4) Checkout — order summary showing ticket types, quantities, tax and total before payment, with a timed hold on the selected seats; 5) Ticket — each ticket its own card with barcode and booking ID, swipeable if bought for friends. Keep the flow to a few taps, prices honest, and the selected seats always visible on the map.",
  "prompt_zh": "活动票务五步：发现（海报+日期+场馆+起价）→详情（单屏+底部固定选座）→选座（分区配色座位图+数量步进+最佳座位推荐+无障碍/视线受限标注）→结账（税费明细+限时锁座）→票据（每张票独立条码卡、可滑动）。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-19T09:12:00+08:00",
  "source": "Ticko 票务 App 案例研究（sigalih.com）+ Showpass《Seating maps and assigned seating》选座地图指南（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-19）"
}
```

## 2026-11-20 · 公开渠道新收集（5 条）

来源核对：5 条原文均已打开核对，按要点改写（非逐字摘录）；与正式库 45 条 + 待验证区 51 条逐一去重，无重复。added_at 统一记本轮时间 2026-11-20T08:10:00+08:00。

### 宠物领养滑动匹配 App (`mobile-pet-adoption-swipe`)

```json
{
  "id": "mobile-pet-adoption-swipe",
  "title": "宠物领养滑动匹配 App",
  "category": "移动端App",
  "styles": [
    "滑动卡片",
    "活泼",
    "图片主导"
  ],
  "scenario": "宠物领养/收容所 App，用左右滑动匹配心仪宠物",
  "prompt": "Design a mobile pet adoption app with a Tinder-style swipe experience: a stack of pet cards, each with a large pet photo, name, age, breed and a short funny one-line bio; drag a card left to pass or right to like — the card flies off with a slight rotation — or use the big heart and cross buttons below the stack. Liked pets go to a Matches tab; when both sides match, show a full-screen 'It's a match!' celebration with confetti and a 'Meet them' button. Add a Super Like star button that sends the card flying upward and marks the pet with a star in Matches. Warm, playful design: cream background, coral and amber accents, rounded 24px cards, friendly rounded type. Include filter chips (dog/cat, age, size) above the stack and a pet detail sheet (temperament, health status, shelter, adoption fee) on tap.",
  "prompt_zh": "宠物领养滑动 App：左右滑动选宠物（照片+名字年龄品种+一句俏皮介绍），右滑喜欢进 Matches、双向匹配弹出庆祝屏，星标超喜欢可上滑飞出；顶部筛选 chips，点卡片看性格/健康/收容所/领养费详情，暖色活泼风。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-20T08:10:00+08:00",
  "source": "Medium《I vibe coded Tinder for dogs in 2 minutes 38 seconds. Here is the exact prompt.》原文提示词核对改写，2026-11-20；https://medium.com/@ezzakyyy/i-vibe-coded-tinder-for-dogs-in-2-minutes-38-seconds-here-is-the-exact-prompt-0fd5d943328e"
}
```

### 在线课程单节课播放页 (`edu-course-lesson-player`)

```json
{
  "id": "edu-course-lesson-player",
  "title": "在线课程单节课播放页",
  "category": "移动端App",
  "styles": [
    "教育",
    "视频播放",
    "学习"
  ],
  "scenario": "在线教育 App 的单节课学习页（视频+笔记+讨论）",
  "prompt": "Design a mobile online-course lesson screen: a 16:9 video player area on top with a large play button overlay, playback speed control and a progress bar with chapter markers; below it the lesson title, course name and instructor with avatar; a progress line 'Lesson 3 of 12' with a thin progress bar; a tab bar with four tabs — Overview, Notes, Resources, Discussion. Overview tab shows the lesson description, 3 key takeaways as bullets and a 'Next lesson' card; Notes tab has a timestamped note editor (tap a timestamp to jump the video); Resources tab lists downloadable files; Discussion tab shows a short Q&A thread. A sticky 'Mark Complete' button sits at the bottom. Clean academic design: white background, one deep-blue accent, readable 16px body text, generous spacing, no decorative gradients.",
  "prompt_zh": "在线课程播放页：16:9 视频区带章节刻度进度条，下方课名/讲师/第 3/12 节进度，概览/笔记/资料/讨论四 tabs（笔记带时间戳可跳视频），底部吸底「标记完成」按钮，干净学术风。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-20T08:10:00+08:00",
  "source": "GenDesigns《The Ultimate AI Design Prompt Library》第 103 条 iOS lesson/lecture screen 原文核对改写，2026-11-20；https://gendesigns.ai/blog/ai-design-prompt-library-100-prompts"
}
```

### 健身房训练记录 App：动作库+组数+休息计时 (`mobile-gym-workout-logger`)

```json
{
  "id": "mobile-gym-workout-logger",
  "title": "健身房训练记录 App：动作库+组数+休息计时",
  "category": "移动端App",
  "styles": [
    "健身",
    "力量训练",
    "深色"
  ],
  "scenario": "力量训练/去健身房时，边练边记录组数次数和组间休息",
  "prompt": "Design a gym workout logger app for strength training: an exercise library screen with categories (Chest, Back, Legs, Arms) and filters, each exercise row showing name, muscle group and a small demo thumbnail; an active workout screen where the current exercise shows a large set table — set number, weight, reps — with tap-to-increment reps and quick weight stepper, a prominent rest timer between sets that counts down from 90s with a circular progress ring and auto-advances to the next set, and a big 'Finish set' button; a session summary with total volume, duration and personal records highlighted; a progress screen with weekly volume bar chart and strength trend lines. Dark theme with electric lime-green accent, huge glanceable numbers (reps/sets/time), minimum 56px tap targets, minimal typing — users are sweating and mid-workout. Distinct from a general health app: this is about logging sets and rest, not daily activity rings or sleep.",
  "prompt_zh": "健身房训练记录：动作库按肌群分类筛选、训练中大字组数表（组/重量/次数点按递增）、90 秒组间休息计时圆环自动进下一组、练后总容量与 PR 汇总、周容量柱状图，深色+荧光绿大字大按钮，出汗时也能单手操作；与库里 mobile-health（日常活动圆环+睡眠）场景不同。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-20T08:10:00+08:00",
  "source": "GenDesigns《Fitness App Design: Workout & Tracker UI with AI》Gym Workout Logger 原文提示词核对改写，2026-11-20；https://gendesigns.ai/design/fitness-app"
}
```

### 房地产看房 App：AI 搜房+约看房 (`mobile-real-estate-viewing`)

```json
{
  "id": "mobile-real-estate-viewing",
  "title": "房地产看房 App：AI 搜房+约看房",
  "category": "移动端App",
  "styles": [
    "房产",
    "图片主导",
    "简洁"
  ],
  "scenario": "找房/买房 App：搜房、看房源详情、预约实地看房",
  "prompt": "Design a mobile real estate app for finding and viewing homes: a photo-led discovery home screen with large property photos, price, bedrooms, area and location on each card, plus filter chips for budget, bedrooms and must-haves and a map toggle that shows listings as pins; an AI-assisted search where the user describes their ideal home in plain words ('quiet, two bedrooms, near a park, under $400k'), the assistant asks one focused follow-up and turns the answer into editable criteria chips the user can review — no unexplained match scores; a property detail screen that presents the essentials first (price, rooms, area, amenities, neighbourhood notes) before a prominent 'Book a viewing' button; a short viewing flow asking for preferred date, time and visit type (in person / video call), ending on a confirmation screen that says the request was sent and the agent still needs to confirm. Warm minimal design: pale surfaces, rounded property cards, one warm-orange accent for primary actions, restrained typography, quiet and trustworthy.",
  "prompt_zh": "房产看房 App：照片主导的房源发现+地图找房、说人话的 AI 搜房（追问一句后转成可编辑的条件 chips，不给玄学匹配分）、详情页先给关键信息再约看房、选日期时间与看房方式后确认待中介回复，米白底+暖橙强调色。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-20T08:10:00+08:00",
  "source": "Luay AlRahahleh《Real Estate App UI/UX — Daira》设计概念原文核对，按要点改写（非逐字摘录），2026-11-20；https://luay.info/daira/"
}
```

### 电商 AR 试穿：商品页试穿入口与试穿屏 (`ecom-ar-tryon-product`)

```json
{
  "id": "ecom-ar-tryon-product",
  "title": "电商 AR 试穿：商品页试穿入口与试穿屏",
  "category": "电商零售",
  "styles": [
    "AR试穿",
    "电商",
    "转化"
  ],
  "scenario": "眼镜/美妆/配饰电商商品页，加 AR 虚拟试穿时",
  "prompt": "Design an e-commerce product page with AR virtual try-on for glasses/cosmetics/accessories: in the product catalog, every try-on-enabled product card carries a visible 'Available for try-on' tag; on the product detail page, a clear high-contrast 'Try it on' button (mirror or brush icon + text, contrast at least 4.5:1) sits within 650px of the top of the screen, below but never overshadowing the 'Add to cart' button; tapping it opens the try-on screen where the product is applied to the live camera view immediately — no extra steps; the try-on screen keeps an 'Add to cart' button with price and size options visible so the user can buy without leaving; below the try-on area show a small recommendation row ('Recommended for you') suggesting the best-fitting products to avoid choice overload. Mobile-first layout, fast-loading compressed 3D assets, trust signals (ratings, returns policy) near the try-on area. Do not present the AR preview as proof of fit — keep the size chart visible.",
  "prompt_zh": "电商 AR 试穿：可试穿商品卡带「可试穿」标签、详情页 650px 内放高对比「试一试」按钮（不抢加购按钮风头）、点开立即上脸不用多余步骤、试穿屏保留加购按钮与价格尺码、下方给少量推荐防选择困难，附尺码表不把预览当合身保证。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-20T08:10:00+08:00",
  "source": "Banuba《Ecommerce UX & UI Design: How AR Try-On Improves Engagement and Sales》试穿 UI 最佳实践原文核对，按要点改写（非逐字摘录），2026-11-20；https://www.banuba.com/blog/ecommerce-ui-design-best-practices-for-augmented-reality"
}
```

## 2026-11-20 · 公开渠道收集（Achraf Arabi 22 风格库 / Medium 加载态实测 / n8n 工作流画布）

来源核对：黏土拟态、Y2K、像素风三条模板已打开 Achraf Arabi《22 website style prompts》原文核对（2026-11-20），按模板要点改写为库内统一格式，非逐字摘录；骨架屏条目据 Medium《Loading Screen UI for AI Builders and Vibe Coders》eBay 骨架屏示例原文提示词核对改写；工作流画布条目据 n8n 官方文档与 Neuraui Flow 组件文档搜索结果核对节点模型，提示词原创，标注「同类收集，非原作摘录」。以上 5 条均为库里没有的风格/场景（黏土拟态、Y2K、像素风、骨架屏加载、智能体工作流画布），其中 3 条落地页风格按 2026-11-17 定规并入已有 landing-styles 风格组作新 variant，只进待验证区。

### 本批新增待验证条目（5 条）

#### 黏土拟态落地页 (`landing-claymorphism`)

```json
{
  "id": "landing-claymorphism",
  "title": "黏土拟态落地页",
  "category": "落地页官网",
  "styles": [
    "黏土拟态",
    "柔和立体",
    "落地页"
  ],
  "scenario": "儿童、游戏、健康类产品落地页想要柔软可触的黏土质感时",
  "prompt": "Design a landing page in Claymorphism style: everything looks like soft, inflated modelling clay you could press with a finger. Layout: a centred hero with one large matte 3D clay object beside the headline, then floating cards with at least 32px of space between them and few elements per section. Type: Fredoka semi-bold for headings (48-72px), Nunito for body, rounded letterforms only. Colour: pale base #F4EEFF, three pastel accents — pink #FFB8D9, mint #A8E6CF, periwinkle #B5C7FF — text in deep plum #2B2340, never pure black; the primary button uses the strongest pastel. Surfaces: corner radius 28-40px on everything; every card uses the same three shadows — a soft drop shadow (0 18px 40px at 18% opacity), an inner highlight at the top left (inset 6px 6px 12px white at 70%) and an inner shade at the bottom right (inset -8px -8px 16px black at 8%); no borders. Images: matte 3D clay renders, one per section, all lit from the same side. Motion: the hero object floats 6-8px on a slow 4-second loop; buttons squash to 96% when pressed and spring back; cards rise 4px on hover. One primary action per screen, body text at least 16px with 4.5:1 contrast, Lucide icons only, no emoji; respect prefers-reduced-motion.",
  "prompt_zh": "黏土拟态落地页：#F4EEFF 淡底+三色粉彩、圆角 28–40px、每张卡同一组三重阴影（外投影+左上内高光+右下内暗角）、无边框，3D 黏土物 4 秒缓浮、按钮按压缩 96% 回弹。",
  "tools": [
    "v0",
    "Lovable",
    "Framer"
  ],
  "group": {
    "id": "landing-styles",
    "name": "落地页官网 · 风格组"
  },
  "variant_label": "黏土拟态",
  "added_at": "2026-11-20T09:15:00+08:00",
  "source": "Achraf Arabi《22 website style prompts》Claymorphism 模板原文核对，按要点改写（非逐字摘录），2026-11-20；https://www.achref.dev/resources/style-prompts"
}
```

#### Y2K 液态铬落地页 (`landing-y2k-chrome`)

```json
{
  "id": "landing-y2k-chrome",
  "title": "Y2K 液态铬落地页",
  "category": "落地页官网",
  "styles": [
    "Y2K",
    "液态铬",
    "复古未来"
  ],
  "scenario": "时尚、美妆、音乐、Z 世代产品落地页想要 2000 年千禧复古未来感时",
  "prompt": "Design a landing page in Y2K aesthetic: the year-2000 internet — glossy bubbles, iridescent stickers, pixel type and pop-up windows. Layout: a playful hero with one big glossy word, sticker elements around it, and content inside retro 'window' frames with blue title bars and small square buttons. Type: Syne extra-bold for headings, DM Sans for body, Silkscreen only for tiny pixel labels and tags. Colour: baby pink #FFB3DE, baby blue #A6D8FF, lilac #CBB6FF, chrome silver and white; iridescent gradients only on stickers, never behind text. Surfaces: glossy pill buttons with a white highlight ellipse on top; sticker shapes (stars, hearts, butterflies) with a white outline. Images: flash-photography portraits and products, chrome hearts and stars, iridescent 3D bubbles. Motion: stickers twinkle and bob in place; buttons bounce on hover; one thin marquee band of text. One primary action per screen, body text at least 16px with 4.5:1 contrast, Lucide icons only, no emoji; respect prefers-reduced-motion.",
  "prompt_zh": "Y2K 液态铬落地页：粉蓝紫+铬银、Syne 粗体标题+Silkscreen 像素小标签、光泽药丸按钮配白色高光椭圆、内容装进复古蓝标题栏窗口、贴纸星星爱心白边闪烁浮动，彩虹渐变只用在贴纸上不垫正文。",
  "tools": [
    "v0",
    "Lovable",
    "Framer"
  ],
  "group": {
    "id": "landing-styles",
    "name": "落地页官网 · 风格组"
  },
  "variant_label": "Y2K液态铬",
  "added_at": "2026-11-20T09:15:00+08:00",
  "source": "Achraf Arabi《22 website style prompts》Y2K Aesthetic 模板原文核对，按要点改写（非逐字摘录），2026-11-20；https://www.achref.dev/resources/style-prompts"
}
```

#### 像素风落地页 (`landing-pixel-art`)

```json
{
  "id": "landing-pixel-art",
  "title": "像素风落地页",
  "category": "落地页官网",
  "styles": [
    "像素风",
    "复古游戏",
    "8-bit"
  ],
  "scenario": "游戏、开发者工具、黑客松、复古品牌落地页想要 8-bit 像素游戏感时",
  "prompt": "Design a landing page in Pixel Art style: an interface straight out of a retro game — chunky pixels, dialog boxes and sprites. Layout: an 8px grid for everything; a hero with a pixel scene and a dialog box carrying the headline; menus styled like game menus; stats shown as health bars. Type: Pixelify Sans for headings, Space Mono for body so long text stays readable; pixel fonts only at their designed sizes, never stretched. Colour: one limited palette of at most 16 colours (for example PICO-8: #1D2B53, #7E2553, #008751, #FFA300, #FFEC27, #29ADFF, #FF77A8, #FFF1E8); no colours outside it. Surfaces: square corners, borders built from 4px pixel steps, buttons with a pixel bevel (light top-left, dark bottom-right); no radius, no blur. Images: pixel sprites and scenes made at a small size and scaled up by whole numbers (2x, 3x, 4x) with image-rendering: pixelated, never smooth-scaled. Motion: the hero sprite plays an idle animation at about 8 frames per second in steps; buttons move 4px down when pressed; dialog text types in letter by letter. One primary action per screen, body text at least 16px with 4.5:1 contrast, Lucide icons only, no emoji; respect prefers-reduced-motion.",
  "prompt_zh": "像素风落地页：8px 网格、PICO-8 限色 16 色内、方角+4px 像素阶梯边框+像素斜面按钮、精灵按整数倍放大（pixelated 不模糊缩放）、主角 8fps 逐帧待机动画、对话框逐字打出。",
  "tools": [
    "v0",
    "Lovable",
    "Framer"
  ],
  "group": {
    "id": "landing-styles",
    "name": "落地页官网 · 风格组"
  },
  "variant_label": "像素风",
  "added_at": "2026-11-20T09:15:00+08:00",
  "source": "Achraf Arabi《22 website style prompts》Pixel Art 模板原文核对，按要点改写（非逐字摘录），2026-11-20；https://www.achref.dev/resources/style-prompts"
}
```

#### 骨架屏加载占位 (`detail-skeleton-loading`)

```json
{
  "id": "detail-skeleton-loading",
  "title": "骨架屏加载占位",
  "category": "细节优化",
  "styles": [
    "骨架屏",
    "加载态",
    "微光"
  ],
  "scenario": "页面数据加载时，不想只转圈、想先露出页面轮廓时",
  "prompt": "Add a skeleton loading state to this page: render the real header, search bar and bottom navigation immediately — only the data-driven parts load. While content is fetching, show skeleton placeholders with the exact layout of the real content: a row of pill-shaped chips, then a grid of rounded image blocks with two short text lines under each, using the same spacing as the real cards. Use a soft shimmer sweep (about 1.4s, left to right, staggered per column by 150ms so it reads as a wave, not a synchronized blink) and swap each placeholder for its real card as data arrives so nothing shifts. If the wait is driven by an AI feature, add a status line with a sparkle icon and a specific message ('Finding the best options...') above a skeleton list that matches the final row layout. Mark the loading region aria-busy='true' and replace the shimmer with a static 60% opacity fill under prefers-reduced-motion. Use a skeleton only when the final shape is known; use a spinner for short actions where the layout does not change.",
  "prompt_zh": "骨架屏加载：先渲染真实页眉/搜索/底栏，只给数据区做与真实内容同尺寸同间距的灰块占位、1.4 秒柔和微光按列错峰扫过、数据一到逐块替换不跳动；AI 任务加一句具体状态文案，减动效时改静态填充。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-20T09:15:00+08:00",
  "source": "Medium《Loading Screen UI for AI Builders and Vibe Coders》eBay 骨架屏示例原文提示词核对，按要点改写（非逐字摘录），2026-11-20；https://medium.com/codetodeploy/loading-screen-ui-for-ai-builders-and-vibe-coders-12-real-app-examples-with-copy-paste-prompts-84d3eefea25d"
}
```

#### AI 智能体工作流画布 (`ai-agent-workflow-canvas`)

```json
{
  "id": "ai-agent-workflow-canvas",
  "title": "AI 智能体工作流画布",
  "category": "AI产品",
  "styles": [
    "工作流画布",
    "节点编辑器",
    "智能体"
  ],
  "scenario": "做 n8n 风格的 AI 智能体工作流搭建器、节点连线画布界面时",
  "prompt": "Design an AI agent workflow builder with a node-based canvas: a large dotted-grid canvas where users drag nodes and connect them with curved edges — Trigger nodes (manual, webhook, schedule, new email) start a flow, Action nodes call models or apps, Logic nodes (IF, Switch, Filter) branch the path, and AI Agent nodes let an LLM plan and call tools. Each AI Agent node shows its sub-nodes underneath: a Chat Model (provider + model picker), an optional Memory node (session-based), and one or more Tool nodes (web search, calculator, email, database). Canvas interactions: pan by dragging empty space, zoom around the pointer, minimap with a draggable viewport box, snap-to-grid, multi-select and group. Running state: each node shows live status (idle / running / done / error) with animated data dots travelling along active edges, plus a side execution log panel listing each step's input and output. Safety: insert a human approval step before any node that sends a message, writes to a database, deletes data or spends money; the run pauses there until approved. Clean light theme, one accent colour for the active path, monospace labels for node types, zoom controls and a 'Test workflow' button in the top bar.",
  "prompt_zh": "AI 智能体工作流画布：触发器/动作/逻辑/AI Agent 节点拖拽连线（Agent 节点下挂模型+记忆+工具子节点），平移缩放+小地图+吸附网格，运行时节点亮状态、数据点沿连线流动、侧栏执行日志，凡发消息/写库/删除/花钱的节点前必须插人工审批。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-20T09:15:00+08:00",
  "source": "同类收集，非原作摘录（节点模型据 n8n 官方文档与 Neuraui Flow 组件文档搜索结果核对，提示词原创，2026-11-20）"
}
```

## 2026-11-21 · 公开渠道收集（番茄钟/习惯打卡/睡眠呼吸/智能手表表盘）

### 番茄钟专注计时：番茄倒计时环+四节进度点 (`mobile-pomodoro-timer`)

```json
{
 "id": "mobile-pomodoro-timer",
 "title": "番茄钟专注计时：番茄倒计时环+四节进度点",
 "category": "效率工具",
 "styles": [
  "专注",
  "番茄钟",
  "效率工具"
 ],
 "scenario": "做专注计时/番茄钟界面，希望倒计时本身就是视觉主角时",
 "prompt": "Design a Pomodoro focus timer widget for a desktop focus app or dashboard corner: a cream card with a 2.5px brown outline and a hard 8px offset shadow, like a sticker. The countdown ring IS the tomato — a thick red ring with a green star-shaped calyx and stem on top at 12 o'clock; the ring empties clockwise as time runs down. Three modes (Focus 25, Short break 5, Long break 15) recolour the ring: tomato red for focus, leaf green for breaks. Four session dots under the controls show progress through a set. First frame mid-session and running: Focus mode, 17:24 remaining, label \"Focus · 2 of 4\", first dot filled, second dot ringed as current, \"Next: short break · 5 min\", \"Today: 50 min focused\". Big centre button toggles Start/Pause.",
 "prompt_zh": "番茄钟计时器：倒计时环本身就是一颗番茄（红色粗环+顶部绿色星形萼片），专注 25/短休 5/长休 15 三档换色，下方 4 个进度点标示一轮进度；奶油卡片+棕色粗描边+硬阴影贴纸风，首帧为专注进行中 17:24。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-21T08:11:00+08:00",
 "source": "Design Lounge《Tomato pomodoro timer widget》brief（2026-11-21 已打开核对原文，按要点改写，非逐字摘录）"
}
```

### 习惯打卡：今日一键打卡+连续记录+热力图 (`mobile-habit-tracker`)

```json
{
 "id": "mobile-habit-tracker",
 "title": "习惯打卡：今日一键打卡+连续记录+热力图",
 "category": "效率工具",
 "styles": [
  "习惯",
  "打卡",
  "连续记录"
 ],
 "scenario": "做习惯养成 App，希望打卡快到打开即点、进度一眼可见时",
 "prompt": "Design a habit tracker app for people building 3 to 5 daily habits. Today screen: a list of today's habits, each with one large tap target (at least 44x44pt) and its current streak with a flame; one tap marks complete with a small satisfying fill animation — no confirmation step. Habit detail screen: current and longest streak, a monthly heatmap calendar of past weeks, completion rate and reminder settings, with three distinguishable states (done / not yet / missed) carried by shape and fill, not colour alone. Add-habit form kept short: name, frequency (every day, specific days, or N times a week), reminder time, optional icon or colour. Weekly stats screen: completion rates and streaks only. Calm and encouraging tone, never shaming; a missed day does not reset progress harshly — offer skip days or a streak freeze.",
 "prompt_zh": "习惯打卡 App：今日页每条习惯一个大号一键打卡目标+连续天数火焰标，打卡有点亮填充小动画无需确认；详情页有月热力图与最长连续记录，未做/未到/漏做三种状态用形状+填充区分而不只靠颜色；语气平静鼓励、不羞辱，漏打卡不粗暴清零。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-21T08:11:00+08:00",
 "source": "Outclass《Habit tracker app design: screens and patterns》+ greta.sh 单提示词（2026-11-21 已打开核对原文，按要点改写，非逐字摘录）"
}
```

### 睡眠呼吸助眠屏：4-7-8 呼吸光球+环形时长拨盘 (`mobile-sleep-breath`)

```json
{
 "id": "mobile-sleep-breath",
 "title": "睡眠呼吸助眠屏：4-7-8 呼吸光球+环形时长拨盘",
 "category": "移动端App",
 "styles": [
  "睡眠",
  "呼吸",
  "助眠"
 ],
 "scenario": "做睡眠 App 的睡前放松屏，希望一屏只做呼吸引导、慢慢淡出时",
 "prompt": "Design the wind-down screen of a sleep app called Hushwell: one rich material — a lit breathing sphere — sits on near-black. The orb swells and shrinks through a 4-7-8 breath (4 seconds in, 7 held, 8 out) and its colours follow the hour: moonlit silver-blue at night, amber at dusk, peach at dawn, pale gold by day. A thin 300° ring around the orb doubles as the session dial: drag its ivory knob from 5 to 45 minutes and the end time updates beneath. Three sound chips (Rain, Brown noise, Harbour). Start lets the chrome dissolve over 1.4 seconds, leaving only the orb, the breath cue, a remaining time and one quiet \"End session\"; in the last stretch the screen, the orb and the sound fade down together. iOS-style restraint: serif italics for the voice, a grotesk for the facts, one primary button. Initial state: 21:30 · Night, dial set to 20 minutes, \"20 min · ends 21:50\", Rain selected.",
 "prompt_zh": "睡眠助眠屏：近黑底上一颗发光呼吸球做 4-7-8 呼吸（吸 4/屏 7/呼 8），颜色随夜/暮/晨/昼变化；球外 300° 细环是时长拨盘（5–45 分钟拖动），配雨声/白噪音/海港三枚音效芯片；开始后界面 1.4 秒淡出只剩呼吸球与剩余时间，结尾一起淡暗。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-21T08:11:00+08:00",
 "source": "Design Lounge《Sleep breath wind-down》brief（2026-11-21 已打开核对原文，按要点改写，非逐字摘录）"
}
```

### 智能手表表盘：Matrix 数字雨+时间电量心率 (`wearable-watchface-matrix`)

```json
{
 "id": "wearable-watchface-matrix",
 "title": "智能手表表盘：Matrix 数字雨+时间电量心率",
 "category": "智能穿戴",
 "styles": [
  "智能穿戴",
  "表盘",
  "赛博"
 ],
 "scenario": "做智能手表表盘，希望一眼可读又有强烈主题氛围时",
 "prompt": "Design a smartwatch face in the style of the Matrix digital rain: green katakana characters pour down the screen in columns from the top, columns starting at random times and falling at different speeds, a white leading character in each column with a tail that fades through three greens. The rain washes away the battery and heart rate readouts as it passes, with the time showing through clearly. Battery icon shows the charge level and a heart icon replaces text labels for heart rate. The rain starts the moment the wrist is raised and runs for as long as the screen stays on. Treat the face as a mini dashboard: keep hierarchy readable at a glance on a small round display (416×416), bold silhouettes, minimal text, strong contrast, no hairline strokes or busy textures.",
 "prompt_zh": "智能手表 Matrix 数字雨表盘：绿色片假名雨柱自顶部落下、各列随机起落速度不一，每列首字白色、尾迹三档绿色渐隐；雨水漫过电量与心率读数、时间始终清晰；电池与心率改用图标而非文字，抬腕即开始下雨。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-21T08:11:00+08:00",
 "source": "the5krunner《How to Make A Garmin Watch Face With Claude》（2026-11-21 已打开核对原文，按要点改写，非逐字摘录）+ CapCut《AI Image for Wearables》表盘可读性要点"
}
```

## 2026-11-21 · 公开渠道收集（第二轮：菜谱详情/订阅追踪/三栏收件箱/先定设计方向/数据表格）

来源核对：菜谱详情、订阅管理、数据表格见 GenDesigns《The Ultimate AI Design Prompt Library: 100+ Copy-Paste Prompts》（2026-11-21 已打开全文核对，#98 菜谱详情、#38 订阅管理、#58 数据表格）；个人订阅追踪见 Medium《Build your subscription tracker with AI in First.new》（搜索结果原文核对：循环付款、续费日历、费用汇总）；三栏收件箱见 Techpresso《30 Claude Prompts That Design UI Screens》Inbox / Messaging 节（搜索结果原文核对）；先定设计方向见 Nebula《Frontend prompt library》所摘 Anthropic 官方 frontend-design Skill（搜索结果原文核对）。以上 5 条均为库里没有的场景/角度（外卖点餐 mobile-food 是下单不是菜谱；mobile-fintech 是通用金融 App 不是订阅追踪；ai-chat-app 是 AI 对话不是三栏收件箱；detail-feizhang-deai-four 是视觉规则、先定方向是生成前的规划步骤；saas-admin-light 是整体管理系统不是数据表格单屏），提示词均按主题原创改写，标注「同类收集，非原作摘录」，只进待验证区。

### 菜谱详情页：大图+配料勾选+步骤分签 (`mobile-recipe-detail`)

```json
{
  "id": "mobile-recipe-detail",
  "title": "菜谱详情页：大图+配料勾选+步骤分签",
  "category": "移动端App",
  "styles": [
    "食谱",
    "菜谱详情",
    "美食"
  ],
  "scenario": "做菜谱/食谱 App 的菜品详情页，希望做菜时能边看边勾选配料时",
  "prompt": "Design an iOS recipe detail screen: a large hero image of the dish at the top, recipe name, author with avatar, stats row (cooking time, servings, difficulty), rating with stars and review count. Tabs below: Ingredients, Instructions, Reviews. The Ingredients tab lists 8 ingredients with checkboxes so the cook can tick items off while shopping or cooking. Save/bookmark and share buttons in the header. Clean, food-focused design with warm appetizing colors, generous spacing, and large readable type for use in the kitchen.",
  "prompt_zh": "菜谱详情页：菜品大图+作者+时长/份量/难度/评分，配料/步骤/评价三签切换，配料带勾选框可边做边打勾，厨房场景下字要大、间距要宽。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-21T09:14:00+08:00",
  "source": "GenDesigns《The Ultimate AI Design Prompt Library》#98 菜谱详情节（2026-11-21 已打开核对原文，按要点改写，同类收集，非原作摘录）"
}
```

### 订阅追踪：续费日历+月度支出汇总 (`mobile-subscription-tracker`)

```json
{
  "id": "mobile-subscription-tracker",
  "title": "订阅追踪：续费日历+月度支出汇总",
  "category": "移动端App",
  "styles": [
    "订阅管理",
    "续费日历",
    "支出汇总"
  ],
  "scenario": "流媒体/会员/软件订阅太多，想一眼看清每月花多少、下一次续费是哪天时",
  "prompt": "Design a personal subscription tracker app: a cost summary card at the top showing total monthly spend and total yearly spend, with a small breakdown by category (streaming, software, fitness, news). Below, a renewal calendar marking each upcoming renewal date with the service logo and amount. The subscription list shows each service with its icon, name, price, billing cycle (monthly/yearly), payment method and renewal date, plus a cancellation status. Include a prominent 'Add subscription' action and a filter by category or billing cycle. Clean, trustworthy design with one accent color; amounts in tabular numerals so totals line up.",
  "prompt_zh": "个人订阅追踪：顶部月/年总支出汇总卡+分类小计，下方续费日历标出每次扣费日期，订阅列表含图标/价格/周期/付款方式/续费日，金额用等宽数字对齐。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-21T09:14:00+08:00",
  "source": "Medium《Build your subscription tracker with AI in First.new》（循环付款、续费日历、费用汇总）+ GenDesigns #38 订阅管理节（搜索结果原文核对，2026-11-21；按主题原创改写，同类收集，非原作摘录）"
}
```

### 三栏收件箱：文件夹+会话列表+阅读窗 (`saas-inbox-three-pane`)

```json
{
  "id": "saas-inbox-three-pane",
  "title": "三栏收件箱：文件夹+会话列表+阅读窗",
  "category": "SaaS后台",
  "styles": [
    "收件箱",
    "三栏布局",
    "消息"
  ],
  "scenario": "做客服/团队收件箱或消息中心，希望文件夹、会话列表、阅读窗三栏并行时",
  "prompt": "Design a three-pane inbox / messaging screen for a support or team workspace: a narrow left rail of folders and filters with unread counts (Inbox, Starred, Assigned to me, Archived), a middle conversation list where each row shows avatar, sender, subject, a one-line preview snippet, timestamp and an unread dot, and a right reading pane showing the selected thread as message bubbles with a reply composer at the bottom. The selected conversation is highlighted in the list; unread rows are bold. Include a search box above the list and a compose button. Clean, dense but scannable layout with subtle dividers, one accent color for the active selection.",
  "prompt_zh": "三栏收件箱：左窄栏文件夹/筛选带未读数，中栏会话列表（头像/发件人/主题/摘要/时间/未读点），右栏阅读窗+底部回复框；选中会话高亮、未读加粗。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-21T09:14:00+08:00",
  "source": "Techpresso《30 Claude Prompts That Design UI Screens》Inbox / Messaging 节（搜索结果原文核对，2026-11-21；按主题原创改写，同类收集，非原作摘录）"
}
```

### 先定设计方向再写代码：主题+配色+字阶+线框 (`detail-design-direction-first`)

```json
{
  "id": "detail-design-direction-first",
  "title": "先定设计方向再写代码：主题+配色+字阶+线框",
  "category": "细节优化",
  "styles": [
    "设计方向",
    "去AI味",
    "方法论"
  ],
  "scenario": "写代码前先让 AI 定设计方向，避免一上来就出通用模板脸时",
  "prompt": "Before writing any code, act as a senior design director and first establish a unique design plan for this project: 1) confirm the core theme and audience; 2) set 4-6 core hex colors; 3) plan the typography and type scale (1-2 curated fonts); 4) describe the layout in one sentence plus a small ASCII wireframe; 5) state the design principles. Strictly avoid common AI default tropes: warm beige with terracotta, black backgrounds with acid green, newspaper-style columns, and SaaS cards with all rounded corners. Only after the plan is agreed, generate the interface from it.",
  "prompt_zh": "生成前先让 AI 当设计总监定方向：主题与受众、4-6 个主色、1-2 款字体与字阶、一句话布局+ASCII 线框、设计原则；并点名避开暖米+陶土、黑底+荧光绿、报纸分栏、全圆角 SaaS 卡等 AI 默认脸。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-21T09:14:00+08:00",
  "source": "Nebula《Frontend prompt library》所摘 Anthropic 官方 frontend-design Skill（搜索结果原文核对，2026-11-21；按主题原创改写，同类收集，非原作摘录）"
}
```

### 数据表格：可排序筛选+多选批量操作 (`saas-data-table`)

```json
{
  "id": "saas-data-table",
  "title": "数据表格：可排序筛选+多选批量操作",
  "category": "SaaS后台",
  "styles": [
    "数据表格",
    "排序筛选",
    "批量操作"
  ],
  "scenario": "后台需要一张能排序、筛选、多选批量处理的数据表时",
  "prompt": "Design a web data table for an admin workspace: a table header with 5 column titles and 5 rows of realistic data. Columns are sortable by clicking the header; rows show a hover state; a checkbox column enables multi-select with a bulk-action bar appearing when rows are selected. Above the table, a search bar and column filters; below, pagination reading 'Showing 1-10 of 234' with page controls. Professional, data-dense design with tabular numerals, sticky header, generous row height for readability, and one accent color for sort indicators and selected states.",
  "prompt_zh": "后台数据表格：5 列可点击表头排序、行悬停、复选框多选后出现批量操作栏，上方搜索+列筛选，下方“显示 1-10 / 共 234 条”分页；等宽数字、吸顶表头、信息密集但可读。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-21T09:14:00+08:00",
  "source": "GenDesigns《The Ultimate AI Design Prompt Library》#58 数据表格节（2026-11-21 已打开核对原文，按要点改写，同类收集，非原作摘录）"
}
```

## 2026-11-22 · 公开渠道收集（打车/天气/新闻/冥想/求职）

### 打车 App：夜间叫车三态 (`mobile-ride-hailing-night`)

```json
{
 "id": "mobile-ride-hailing-night",
 "title": "打车 App：夜间叫车三态",
 "category": "移动端App",
 "styles": [
  "深色",
  "地图主导",
  "底部面板"
 ],
 "scenario": "打车/共享出行 App 叫车主界面（选车→找司机→司机已接单）",
 "prompt": "Design a night ride-hailing app screen (390x844): a near-black map fills the whole phone with a dashed acid-yellow route from a white ring pickup pin to a yellow square destination pin, and a small '18 MIN' trip-time tag on the drop pin. A flat dark bottom sheet holds two place rows in one box (Pickup / Destination) with a 44px swap button that rotates 180° when tapped, three ride options as a radio group (Moto 3 min · 1 seat $6.40, Car 5 min · 4 seats $11.80 selected, XL 9 min · 6 seats $17.20) each showing wait time, seats and price in monospace, a payment row (VISA ···· 4417 · Change), and one big acid-yellow button whose label names the selected ride ('Request Car' becomes 'Request XL' when XL is picked). Include the three states: plan, finding (radar rings spreading from the pickup pin, progress bar, 'Finding your driver', Cancel), and found (driver card with photo, name, 4.92 rating, trips count, plate in large mono like a real plate, Message/Call buttons). Industrial night look: near-black greys #0d0e0f/#121314, white type, one acid accent #d7ff2e, condensed caps for names, IBM Plex Mono for every number, 8px corners, 1px hairlines, no shadows, no glass. Hit targets 44px or larger.",
 "prompt_zh": "夜间打车主界面：近黑地图+酸黄虚线路线、上下车点可互换、三档车型单选、主按钮文案跟着选中车型变，含选车/找司机/已接单三态与司机卡片车牌。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T08:10:00+08:00",
 "source": "Design Lounge《Phone ride request》（https://www.designlounge.live/p/phone-ride-request，已打开页面核对原文全文；提示词按其设计简报要点原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

### 天气 App：全屏动态天空+玻璃数据卡 (`mobile-weather-app`)

```json
{
 "id": "mobile-weather-app",
 "title": "天气 App：全屏动态天空+玻璃数据卡",
 "category": "移动端App",
 "styles": [
  "沉浸",
  "玻璃拟态",
  "数据可视化"
 ],
 "scenario": "天气 App 首页（当前天气+逐小时+10 日预报+指标网格）",
 "prompt": "Design a polished native-style weather app home screen (390x844): a full-screen animated sky fills the background behind everything (rain streaks, sun glow, drifting clouds, snowflakes or a starry night, matched to the condition). Centered header with the city name, a huge thin temperature (100pt, e.g. 48°), the condition word and H/L range; the header collapses on scroll to a compact pinned line '48° | Rain'. Below, a glass Conditions card (20pt corners, thin white border) with a 24-column hourly row (hour, weather icon, precipitation % in blue when ≥30%, temperature), a next-hour precipitation bar chart when it is raining, a 10-day forecast card with one row per day (day, icon, low, a temperature-range bar filled with a cold-to-hot gradient, high), and a 2-column grid of square glass tiles: UV index, sunset curve, wind compass, precipitation, feels like, humidity, visibility, pressure — each with an icon header, one big value and a one-line caption. Bottom bar: a glass map circle left, a page-dot capsule in the centre, a glass list circle right. White text, glass cards over a sky-tinted background, one accent color per sky, springy 300ms transitions, pressed states scale 0.97. Include a locations list screen (live mini-sky cards per city with temperature and H/L) and a day-detail sheet with a 24-hour temperature line chart.",
 "prompt_zh": "天气 App 首页：全屏动态天空背景、超大细体温度、玻璃质感逐小时卡片、10 日温度区间条、UV/日落/风速等指标玻璃格，滚动时标题收起。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T08:10:00+08:00",
 "source": "Vibecode《Apple Weather Clone》（https://www.vibecodeapp.com/templates/apple-weather，已打开页面核对原文全文；原文为 2845 词 SwiftUI 专属构建提示词，本条按其结构与视觉要点改写为通用 UI 提示词，同类收集，非原作摘录，2026-11-22）"
}
```

### 新闻资讯 App：纸感头版+离线收藏 (`mobile-news-reader`)

```json
{
 "id": "mobile-news-reader",
 "title": "新闻资讯 App：纸感头版+离线收藏",
 "category": "移动端App",
 "styles": [
  "纸感",
  "衬线标题",
  "编辑排版"
 ],
 "scenario": "新闻资讯 App 首页（头条卡片+栏目筛选+文章列表+离线收藏）",
 "prompt": "Design a news app front page (390x844) with a paper-toned editorial look: cream paper background #FAF6EE, a 30px serif masthead with the date, a horizontally scrolling row of section chips (Top stories, World, Climate, Technology, Culture, Sport) with the pressed chip filled dark ink and the rest outlined. A lead card with a CSS-drawn landscape illustration (gradient sky, sun disc, two hills, no photos), a red kicker, a 26px serif headline, a one-line dek, and a meta line with author, reading time and a green 'saved' mark. Below, a 'Latest' section label and a hairline-separated story list of six stories: 72px thumbnail, 17px serif headline, meta line with section and reading time, and a 40px round bookmark button on the right; saved stories show '· saved' in green inside the meta line (not a separate icon column) and update the badge on the Saved tab. Bottom nav with four items (Today, Sections, Saved with count badge, Me), 64px tall. Serif headlines (Newsreader/Georgia), Inter for UI text, one red accent #A83A2A plus one green #2F6B4F for saved state only, hairlines instead of cards, 280ms dip animation when switching sections, focus rings visible, no horizontal scroll.",
 "prompt_zh": "新闻头版：米白纸感底、30px 衬线刊头、横滑栏目 chips、纯 CSS 风景头条卡、细线分隔的文章列表，收藏状态直接写进元信息行并同步更新 Saved 角标。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T08:10:00+08:00",
 "source": "Design Lounge《PWA news reader》（https://www.designlounge.live/p/pwa-news-reader，已打开页面核对原文全文；提示词按其设计简报要点原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

### 冥想/正念 App：今日一课+呼吸播放器 (`mobile-meditation-app`)

```json
{
 "id": "mobile-meditation-app",
 "title": "冥想/正念 App：今日一课+呼吸播放器",
 "category": "移动端App",
 "styles": [
  "治愈",
  "低饱和",
  "留白"
 ],
 "scenario": "冥想/正念 App（目标选择→今日推荐→播放→完成→进度）",
 "prompt": "Design a 7-screen iOS meditation app (393x852): Welcome (one breathing animation and the line 'Let's take a minute for you'), Goal picker (4-6 large tappable goal chips: sleep, stress, focus, anxiety, habit), Home/Today (time-aware greeting, one hero 'Today's session' card with artwork, duration and a single play button, a small streak/minutes row, 3-5 quick picks like '1-minute breath', and a 'Day 4 of 10' continue-course card), Session detail (title, teacher, 5/10/20-minute duration selector, description, download), Player (one huge ≥64pt play/pause button centred and reachable without looking, a slow progress ring or breathing circle, skip back 15s, timer, ambient-sound volume slider in a sheet, no bright flashes), Completion (calm animation, minutes added, optional mood check-in), Progress (mindful days per week instead of punishing streaks, total minutes, calendar). Warm off-white #F7F4EE background, soft sage #E3EBE3 surfaces, muted teal #2F7D78 primary action, dark navy #0F1729 sleep theme; rounded humanist sans, 34pt large title, 22pt section titles, 17pt body; 20-24pt side margins, 16-24pt card radii, slow ease-in-out motion ≥400ms for ambient elements, breathing animation timed to real breath cycles, Reduce Motion fallback to gentle fades, 44pt minimum tap targets. Get the user into their first session within about a minute of opening the app; defer account creation, reminders and payment until after the first completed session.",
 "prompt_zh": "冥想 App 全套 7 屏：呼吸欢迎页→目标选择→今日一课主卡+温和打卡→可闭眼操作的超大播放键呼吸播放器→完成心情签到→按周统计进度，暖白+鼠尾草+深夜藏青睡眠主题。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T08:10:00+08:00",
 "source": "floow.design《Meditation App Design: Screens, Flows and UI Patterns》（https://www.floow.design/blog/how-to-design-a-meditation-app，已打开页面核对原文全文；提示词按其屏幕清单、三条流程与 MVP 规格原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

### 求职 App：薪资前置的职位列表首页 (`mobile-job-search-home`)

```json
{
 "id": "mobile-job-search-home",
 "title": "求职 App：薪资前置的职位列表首页",
 "category": "移动端App",
 "styles": [
  "列表",
  "信息层级",
  "极简"
 ],
 "scenario": "求职/招聘 App 首页（搜索+筛选+最佳匹配+职位列表）",
 "prompt": "Design a job search app home screen (390x844) built around one rule: the number candidates compare — pay — must be visible in the list, never hidden behind a tap. Top: wordmark and a line '12 new jobs for you', then ONE 44px search field (radius 10, #F2F2F2 fill) reading 'Product designer, remote' with a filter icon inside; category, part-time, entry-level and sort live behind that filter icon, not on screen. Below, a horizontally swiping row of 32px filter chips (Remote, Full-time, $100k+, Easy Apply) with the active filter filled in ink so the current state is obvious, the last chip cut off by the screen edge as the swipe cue. Then the best match gets its own block: 48px logo tile, 16px job title, company and place, the pay range in bold at the same weight as the title (e.g. $120k–$150k), a violet 96% match line, and one full-width Easy Apply button beside a Save bookmark. Every other job is a flat three-line row separated by a hairline: title, company and place, pay range in bold — one bookmark only, no Apply button per row. One margin (20px both sides), one violet accent #5D2EEA used for the wordmark, Easy Apply, the match line and the active tab only; no cards, no shadows, no photos; logos are plain letter tiles radius 8; a four-tab bar in one icon style with a hairline. The sale offer is a single text row under the list ('Try Premium, 50% off'), never a banner above the results.",
 "prompt_zh": "求职首页：一个搜索框+横滑筛选 chips、最佳匹配单独成块带薪资与一键申请、其余职位三行扁平列表且每行都明码标薪，一个边距、一个紫色强调色、无卡片无阴影。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T08:10:00+08:00",
 "source": "Brainy《Job Search App Design: Home Screen Before and After》（http://brainy.ink/paper/job-search-app-design，已打开页面核对原文全文；提示词按其改版前后四条规则与测量值原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

来源核对：打车三态见 Design Lounge《Phone ride request》、天气 App 见 Vibecode《Apple Weather Clone》、新闻头版见 Design Lounge《PWA news reader》、冥想 App 见 floow.design《Meditation App Design》、求职首页见 Brainy《Job Search App Design: Home Screen Before and After》，5 个来源页面均于 2026-11-22 已打开全文核对；提示词均按主题原创改写，标注「同类收集，非原作摘录」，只进待验证区。去重说明：记账/预算与正式库 mobile-fintech（钱包/记账/理财 App 首页）同场景已跳过；民宿预订与待验证区 mobile-travel-booking（旅行预订）场景相近已跳过；新闻头版与待验证区 content-blog-reading（单篇博客阅读页）场景不同、睡眠呼吸单屏与冥想 App 全套流程场景不同，均保留。

### 语言学习 App：游戏化课程路径+爱心/XP (`mobile-language-learning`)

```json
{
 "id": "mobile-language-learning",
 "title": "语言学习 App：游戏化课程路径+爱心/XP",
 "category": "移动端App",
 "styles": [
  "游戏化",
  "明亮活泼",
  "圆润"
 ],
 "scenario": "语言学习 App 首页（课程路径+连胜+爱心/XP）与课堂练习（四选一+单词拼句）",
 "prompt": "Design a gamified language learning app (390x844) with a bright, playful look and its own name, mascot, colours and logo — do not copy any existing brand. Home: a winding lesson path of five gold and green nodes down the screen, a bouncing START bubble on the current node, a locked chest and a trophy at the end; a top bar with a flame streak counter (e.g. 27 days), three hearts and an XP total. A daily goal ring at the top fills up as XP is earned today and resets each day. A lesson has eight exercises of two kinds only: pick the right translation from four choices, and build the sentence by tapping word tiles that fly from the bank to the answer line in 0.3s. After each answer show a full-width green or red feedback bar ('Nice job!' / correct answer) with a CHECK button; a wrong answer costs one heart, and losing all hearts opens a refill-and-retry screen instead of a dead end. Finish with a celebration screen: TOTAL XP, AMAZING and SPEEDY boxes, the flame lighting up as the streak rolls from 27 to 28. Rounded bold type (Nunito or similar), 52px minimum tap targets, lime green for correct, soft red for wrong, one purple for XP and one orange for streak — colour always means the same thing. Progress saves locally so a reload keeps streak, hearts and XP.",
 "prompt_zh": "语言学习 App：蜿蜒金绿课程路径+连胜火焰+爱心/XP，每课 8 道四选一与单词拼句练习，词块 0.3 秒飞入答案行，答错扣爱心、通关点亮连胜火焰，附每日 XP 目标环。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T09:20:00+08:00",
 "source": "Medium Ezzaky Ab.《I vibe coded my own Duolingo with one prompt》（https://medium.com/@ezzakyyy/i-vibe-coded-my-own-duolingo-with-one-prompt-streaks-hearts-and-a-party-at-the-end-for-6-cents-b00cd92d3929，已打开页面核对原文全文；提示词按其一句话提示词与三条生效要点原创改写为通用 UI 提示词，同类收集，非原作摘录，2026-11-22）"
}
```

### 充电桩查找 App：三态应急/计划/旅途+可靠度优先 (`mobile-ev-charging-finder`)

```json
{
 "id": "mobile-ev-charging-finder",
 "title": "充电桩查找 App：三态应急/计划/旅途+可靠度优先",
 "category": "移动端App",
 "styles": [
  "高对比",
  "地图",
  "应急优先"
 ],
 "scenario": "电动车充电桩查找 App（地图+列表：应急找桩/计划停靠/旅途规划）",
 "prompt": "Design an EV charging finder app (390x844) built for high-stress outdoor use: one interface that adapts to three mental states. Emergency mode (battery 5-20%): the nearest WORKING charger wins — one huge 'Navigate to nearest available' action, distance and live availability first, decision in 5 seconds. Planned stop (20-50%): compare speed, price per kWh and reliability side by side, with a 'Recommended' badge that ends choice paralysis and a 'Filling fast' urgency note. Road trip (50%+): route integration with corridor fast chargers, amenities and ratings. Every charger shows reliability, not just location: live free/total port count (e.g. 3 of 4 free), connector types (CCS2, Type 2), price, and a four-lightning-bolt availability pattern (⚡⚡⚡⚡❌) readable in half a second. Map pins and list rows share one availability colour system; colour is reserved for meaning only — green safe, orange urgency, black action, nothing decorative. 56px tap targets, per-card actions instead of a sticky button (the sticky button wastes map space), high contrast for sunlight readability, filter by connector type so no one arrives at the wrong plug. Black/white/green/orange palette only, no decorative colour.",
 "prompt_zh": "充电桩查找 App：应急 5 秒直达最近可用桩、计划停靠比价比可靠度、旅途规划看配套设施，可靠度（空闲桩数/接口/电价）优先于位置，56px 大触区、颜色只表意。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T09:20:00+08:00",
 "source": "Anna Foltman《EV Charging Finder》（https://www.annafoltman.pl/projects/ev-charging.html，已打开页面核对原文全文；提示词按其三态用例、三条设计原则与关键决策原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

### 咖啡点单 App：自提卡+积分进度+行式菜单 (`mobile-coffee-order`)

```json
{
 "id": "mobile-coffee-order",
 "title": "咖啡点单 App：自提卡+积分进度+行式菜单",
 "category": "移动端App",
 "styles": [
  "暖色",
  "奶油底",
  "行式列表"
 ],
 "scenario": "咖啡点单 App 首页（自提门店+积分进度+分类+热门单品）",
 "prompt": "Design a coffee ordering app home screen (390x844) on a cream ground #F5EFE4 where one thing is read per block and one action per row. Top: a large 'Good morning, Leo' greeting with a round bell button, then ONE pickup card: 'Pickup at Downtown' as the title, one grey line '0.3 mi · Open until 9 pm' beneath it, and a blue 'Change' link at the right — the street address is not on the home screen. Below, one deep blue rewards card: 'Rewards' and '1,250 points' on top, the large line '250 points to a free drink', a butter progress bar filled 83% (1,250 of 1,500), and a small line 'A free drink at 1,500 points' — show the distance to the reward, not just the balance. Category row: exactly four chips that fit on screen (All, Coffee, Cold drinks, Bakery), the selected one filled cafe blue with white text; the rest of the menu lives one tap away in the Menu tab. Popular items are rows, not a grid: each row has a 60px photo, name, one grey line and price, with ONE round blue '+' button (44pt tap target) at the right — when every item has the same action, the action stays small and aligned so names and prices line up on one edge. One 20px side margin, 16px between blocks, iOS type scale 11-28pt, four-tab bar (Home, Menu, Rewards, Account). Palette of four only: cafe cobalt #2342A8, deep blue #15276B, butter #F3C77A, cream #F5EFE4; no gradients, no shouting banners.",
 "prompt_zh": "咖啡点单首页：自提门店一张卡+积分进度讲清离免费饮品还差多少、恰好放得下的 4 个分类 chips、热门单品用 60px 图行式列表配单个圆形加号键，奶油底+钴蓝+黄油四色。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T09:20:00+08:00",
 "source": "Brainy《Coffee App Design: Order Home Screen Before and After》（https://brainy.ink/paper/coffee-app-design，已打开页面核对原文全文；提示词按其四项改版规则与测量值原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

### 在线会议工具：主讲/网格视频+聊天/实时摘要/时间轴 (`saas-video-meeting`)

```json
{
 "id": "saas-video-meeting",
 "title": "在线会议工具：主讲/网格视频+聊天/实时摘要/时间轴",
 "category": "SaaS后台",
 "styles": [
  "极简",
  "浅色",
  "圆角"
 ],
 "scenario": "在线会议工具主会议页（视频区+右侧聊天/摘要+底部时间轴）",
 "prompt": "Design a modern online meeting tool main page (1440x900, responsive to mobile) in a minimalist light style: white and soft greys with one blue or green accent, soft shadows and rounded corners. Central area: the video feed, scalable between single-speaker view and a multi-participant tile grid; a floating control bar at the bottom of the video with mute/unmute, camera on/off, screen share and leave — the red leave button visually separated from the rest. Right side: a collapsible sidebar split into two tabs, Participants (avatar, name, mic state, per-person menu for mute/remove/roles, invited-but-not-joined listed separately) and Chat (message history with smooth scrolling, text, emoji and links). Directly below the chat, a live summary panel that updates in real time with the key points being discussed, expandable for detail and collapsible to keep the interface clean. Along the very bottom, a thin full-width timeline bar: a current-time marker draggable to rewind or fast-forward, a 'Now' button on the right to jump back to the live moment, small markers on key moments, and a hover tooltip showing time and the key event summary; scrubbing the timeline highlights the chat messages from that point in time. Non-intrusive toast notifications for new chat messages and important updates only. Every panel visually distinct, nothing competing with the video.",
 "prompt_zh": "在线会议主页面：中央视频主讲/网格切换+底部悬浮控制条，右侧参与者/聊天双标签栏配实时要点摘要，底部可拖动时间轴带关键时刻标记与 Now 回到直播按钮。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T09:20:00+08:00",
 "source": "PureCode《Online Meeting Tool》（https://purecode.ai/community/onlinemeetingtoolui-tailwind-meetingui，已打开页面核对原文全文；提示词按其视频区、聊天、摘要、时间轴四部分规格原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

### 深色模式：语义 token+三级亮面+去饱和强调色 (`detail-dark-mode-tokens`)

```json
{
 "id": "detail-dark-mode-tokens",
 "title": "深色模式：语义 token+三级亮面+去饱和强调色",
 "category": "细节优化",
 "styles": [
  "深色模式",
  "设计系统",
  "无障碍"
 ],
 "scenario": "深色模式配色系统（语义 token 表 + 仪表盘示例，浅/深双主题切换）",
 "prompt": "Design a dark mode analytics dashboard for a SaaS product (1440x900) that demonstrates a proper dark theme token system — dark mode is a second palette, never an inverted one. Base: dark grey #121212 page (never pure black — #fff on #000 hits 21:1 and causes halation), elevation tiers #1e1e1e cards and #2a2a2a dropdowns/modals; elevation comes from lighter surfaces, not shadows. Text: off-white #e6e6e6 primary (15.0:1), #a3a3a3 secondary (7.4:1); disabled text #6b6b6b (3.5:1) is reserved for genuinely disabled states and must never carry real content. One desaturated accent only — take the light-mode 500-weight brand colour and ship its 300-400 weight on dark (e.g. #8ab4f8, 8.9:1); fully saturated hues vibrate against dark surfaces. Borders are 1px rgba(255,255,255,0.12) instead of heavy shadows. Name colours by role, not value: components use --bg, --surface, --raised, --ink, --muted, --line, --accent, and each theme assigns values to those roles. Check contrast in BOTH themes (4.5:1 body text, 3:1 UI components) and test secondary text against the lightest elevated surface --surface-3, not the page background — opacity-based muted text silently fails on raised surfaces. Show the same dashboard in light and dark side by side with a theme toggle, and a small token sheet listing each token with its computed contrast ratio. Never ship filter: invert(1) as dark mode.",
 "prompt_zh": "深色模式配色系统：#121212 底+三级亮面分层、#e6e6e6/#a3a3a3 两级文字、去饱和单一强调色、按角色命名的语义 token，双主题对照并附实测对比度数值表。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-22T09:20:00+08:00",
 "source": "Superdesign《Dark Mode UI: Token Sheet With Computed Contrast, Examples and Limits》（https://superdesign.dev/styles/dark-mode，已打开页面核对原文全文；提示词按其 token 表、对比度数值与强调色规则原创改写，同类收集，非原作摘录，2026-11-22）"
}
```

来源核对：语言学习见 Medium Ezzaky Ab.《I vibe coded my own Duolingo with one prompt》、充电桩查找见 Anna Foltman《EV Charging Finder》、咖啡点单见 Brainy《Coffee App Design》、在线会议见 PureCode《Online Meeting Tool》、深色模式见 Superdesign《Dark Mode UI》，5 个来源页面均于 2026-11-22 已打开全文核对；提示词均按主题原创改写，标注「同类收集，非原作摘录」，只进待验证区。去重说明：咖啡点单与正式库 mobile-food（外卖 App）场景不同（自提咖啡点单 vs 外卖点餐）保留；语言学习与正式库 edu-course-lesson-player（课程播放器）场景不同保留；深色模式与正式库 detail-contrast-a11y（对比度与可读性）角度不同（token 系统 vs 单项对比度）保留；充电桩与在线会议在正式库与待验证区均无同场景条目。

## 2026-11-23 · 公开渠道收集（交友滑动/在线考试/生鲜配送/家政预约/共享单车）

### 交友 App 滑动卡组与匹配页 (`mobile-dating-swipe`)

```json
{
 "id": "mobile-dating-swipe",
 "title": "交友 App 滑动卡组与匹配页",
 "category": "移动端App",
 "styles": [
  "社交",
  "卡片滑动",
  "动效"
 ],
 "scenario": "做交友/婚恋 App 的滑动匹配卡片组时（动效类）",
 "prompt": "Design the Discover tab of a dating app as a swipeable card deck (390x844): a stack of full-bleed profile photo cards, each with a cream info plate at the bottom holding name, age, job, distance and one personality prompt with its answer. Dragging the top card tilts it around a low pivot (up to ±16°), a LIKE or PASS stamp inks in with drag distance, and the next card grows from 0.95 to 1 beneath it. A fast flick flings the card off at release velocity; a slow short drag springs it home over 420ms. Tapping the right half of the photo steps to the next photo, the left half goes back. Liking the third profile opens a calm match screen: two round photos sliding in, 'It's mutual', a message field and a keep-browsing button — no countdowns, no likes-left counter. Below the deck, three round action buttons: Pass (64px), Super Like (52px), Like (64px). iOS-style language: 26px card radius, 44px round header buttons, spring motion, one sans family.",
 "prompt_zh": "交友 App 滑动卡组：全幅照片卡+底部信息板，拖动倾斜±16°、LIKE/PASS 印章随距离显现、下一张卡由 0.95 放大，快甩按速度飞出、慢拖 420ms 回弹，点照片左右半区切换照片，第三张喜欢后开安静匹配页，底部 Pass/Super Like/Like 三钮。动效类，验证需 GIF。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T08:10:00+08:00",
 "source": "Design Lounge《Dating swipe deck with match screen》（https://www.designlounge.live/p/app-dating-swipe-deck，已打开页面核对简报全文；提示词按其卡片物理、印章、匹配页规格原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

### 在线直播刷题 QuizFlix：房间码+分屏白板 (`edu-live-quiz`)

```json
{
 "id": "edu-live-quiz",
 "title": "在线直播刷题 QuizFlix：房间码+分屏白板",
 "category": "移动端App",
 "styles": [
  "教育",
  "直播答题",
  "极简"
 ],
 "scenario": "做大学生直播刷题/考试练习 App 时",
 "prompt": "Design QuizFlix, a mobile live-quiz app for university students: join a quiz by entering a room code, no host required. Timed multiple-choice questions with real-time scoring and a live leaderboard. Split-screen layout — the question on top, a personal whiteboard below for solving problems independently (pen, eraser, undo; local only, never shared), swiping up expands the whiteboard. Minimalist design to keep focus. Real-time sync via Firebase or WebSocket for rooms, questions, answers and scores. Target academic reinforcement and exam practice; keep the MVP to live participation, the whiteboard and the leaderboard.",
 "prompt_zh": "大学生直播刷题 App：房间码入场、无主持人，计时选择题+实时计分与排行榜，上题下白板分屏（画笔/橡皮/撤销、仅本地、上滑展开），极简专注风。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T08:10:00+08:00",
 "source": "Kaushik Sarkar《From One Prompt to a Live QuizFlix Mobile App Design for Uni》转引 prompts.chat 原提示词（https://www.kaushiksarkar.com/blog/from-one-prompt-to-a-live-quizflix-mobile-app-design-for-university-students-sit，已打开页面核对原文全文；提示词按原文要点改写，同类收集，非原作摘录，2026-11-23）"
}
```

### 生鲜配送 App：多店+替换选择+小费 (`mobile-grocery-delivery`)

```json
{
 "id": "mobile-grocery-delivery",
 "title": "生鲜配送 App：多店+替换选择+小费",
 "category": "电商零售",
 "styles": [
  "生鲜",
  "多店铺",
  "配送"
 ],
 "scenario": "做生鲜/超市配送 App 的选店到收货全流程时",
 "prompt": "Design a grocery delivery app covering the full flow from choosing a store to groceries at the door: multi-store home with search across products, stores and recipes, an active-order banner, and store cards showing delivery times and pickup tags. Storefront with a delivery/pickup/in-store toggle, service fee stated up front, flyer deals and an aisle list from Produce to Pets. Search with brand, sale and sort filters; product pages with unit price, stock level and a nutrition panel. Cart where every line carries a replacement choice (Replace with best match, a specific item, or a refund) plus a note field, a fee summary and a spend-more offer for free delivery. Checkout with a dedicated tip screen ($1–$6 presets, the shopper keeps the whole tip), then order tracking with the shopper's profile. Clean, friendly, grocery-fresh visual language.",
 "prompt_zh": "生鲜配送全流程：多店首页+按过道浏览+商品营养信息，每件商品带缺货替换选择，购物车含费用明细与免邮凑单，独立小费页，订单跟踪配采购员信息。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T08:10:00+08:00",
 "source": "Whimsical《Grocery Delivery App Wireframe》（https://whimsical.com/templates/grocery-delivery-app-wireframe，已打开页面核对 15 屏线框图内容；提示词按其 Instacart 流程要点原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

### 家政保洁预约 App：冬季大扫除 (`mobile-home-cleaning-booking`)

```json
{
 "id": "mobile-home-cleaning-booking",
 "title": "家政保洁预约 App：冬季大扫除",
 "category": "移动端App",
 "styles": [
  "家政",
  "预约",
  "暖色"
 ],
 "scenario": "做上门保洁/家政服务预约 App 时",
 "prompt": "Design a mobile home-cleaning booking app screen (portrait phone, soft warm cream background): a deep teal header with the white title 'Book a Winter Cleaning' and a small snowflake icon, a search bar reading 'Search cleaning, laundry, tidying'. Below, a horizontal row of service chips — Deep Clean, Kitchen, Bathroom, Laundry — with Deep Clean selected in teal. A large featured card shows a bright photo of a tidy living room, 'Deep Clean · 2 hours', price '$59', and a teal 'Book Now' button. Below it, a time-slot row with 'Today 2:00 PM' selected, and a cleaner profile row with a friendly avatar, the name 'Ava', 4.9 stars and '128 jobs done'. Bottom navigation: Home, Bookings, Messages, Profile. Short readable English labels only, generous spacing, deep teal and warm cream palette, crisp modern UI.",
 "prompt_zh": "家政保洁预约页：深青+暖米配色，服务 chips（深度清洁/厨房/浴室/洗衣），大卡片配 2 小时 $59 与 Book Now，时间段选择+保洁员 Ava 4.9 星 128 单，底部四栏导航。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T08:10:00+08:00",
 "source": "MyPrompt《Winter Home Cleaning Booking App Interface Prompt》（https://myprompt.cc/en/prompt/winter-home-cleaning-booking-app-interface-prompt-cmwfqp5e，已打开页面核对提示词原文全文；提示词按原文要点改写，同类收集，非原作摘录，2026-11-23）"
}
```

### 共享单车 App：站点地图+扫码开锁 (`mobile-bike-sharing`)

```json
{
 "id": "mobile-bike-sharing",
 "title": "共享单车 App：站点地图+扫码开锁",
 "category": "移动端App",
 "styles": [
  "出行",
  "地图",
  "扫码"
 ],
 "scenario": "做共享单车/城市骑行 App 的找车开锁还车流程时",
 "prompt": "Design a bike-sharing app around the rider's journey: a map home screen showing nearby stations, highlighting only stations with available bikes when location is shared, and hiding empty ones. Tapping a station shows the number of available bikes and the rate per minute so riders can compare by proximity, price and availability. Accepting a rate reserves a bike at that station (no need to pick a specific bike yet, and no need to be at the station to start). To unlock, the rider scans the QR code on the station hardware to prove presence; the station then assigns and unlocks a specific bike. During the ride show live time, distance and cost. To end, the rider returns the bike to a station slot, the hardware locks it and the ride stops, price is calculated and credits deducted, with clear feedback at every step (unlock success/failure, return confirmation) and graceful handling when a lock fails or a bike is defective. Clean map-first design with strong availability and price transparency.",
 "prompt_zh": "共享单车全流程：地图首页只显示有车站点、点站看余量与每分钟价，接受价格即预留，到站扫码开锁，骑行中显示时间里程费用，还车落锁计费扣款，全程状态反馈明确。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T08:10:00+08:00",
 "source": "Gistly《Deep Dive into Bike Sharing App User Flow & Domain Model》（https://gist.ly/youtube-summarizer/deep-dive-into-bike-sharing-app-user-flow-domain-model，已打开页面核对用户旅程全文；提示词按其找车/预留/扫码开锁/还车计费流程原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

来源核对：交友滑动见 Design Lounge 卡片滑动简报、在线考试见 Kaushik Sarkar 转引 prompts.chat 的 QuizFlix 全文提示词、生鲜配送见 Whimsical Instacart 15 屏线框图、家政预约见 MyPrompt 冬季保洁预约提示词原文、共享单车见 Gistly 单车用户旅程深挖，5 个来源页面均于 2026-11-23 已打开全文核对；提示词均按主题原创改写，标注「同类收集，非原作摘录」，只进待验证区。去重说明：交友滑动与待验证区 mobile-pet-adoption-swipe 同为滑动卡片但场景不同（交友 vs 宠物领养）保留；在线考试与正式库 edu-course-lesson-player（课程播放页）场景不同保留；生鲜配送与正式库 mobile-food（外卖点餐）场景不同（多店生鲜采购 vs 单店外卖）保留；家政预约与共享单车在正式库与待验证区均无同场景条目。
