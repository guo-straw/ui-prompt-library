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
  "source_video": "https://www.douyin.com/video/7680742171204439296",
  "verify_note": "2026-11-24 尝试验证：浏览器实测来源视频可正常播放，内容与提示词要点逐条一致，但抖音网页未提供下载途径、无法取得视频文件或直接播放地址（Argus 签名拦截），无法截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7699199951179418907",
  "verify_note": "2026-11-24 尝试验证：浏览器实测来源视频可正常播放，内容与提示词要点逐条一致，但抖音网页未提供下载途径、无法取得视频文件或直接播放地址（Argus 签名拦截），无法截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7682010730085862696",
  "verify_note": "2026-11-24 尝试验证：浏览器实测来源视频可正常播放，内容与提示词要点逐条一致，但抖音网页未提供下载途径、无法取得视频文件或直接播放地址（Argus 签名拦截），无法截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7682681851068026152",
  "verify_note": "2026-11-24 尝试验证：浏览器实测来源视频可正常播放，内容与提示词要点逐条一致，但抖音网页未提供下载途径、无法取得视频文件或直接播放地址（Argus 签名拦截），无法截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7680037853694381327",
  "verify_note": "2026-11-26 复核：仍留待验证——与 2026-11-24 同批 4 条同一阻塞（抖音网页可播放、内容一致，但无下载途径、无法取得视频文件或直接播放地址，无法截取 GIF/关键帧）；本轮未重复尝试下载，待用户从手机抖音 App 保存视频文件后补验；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7687151464640220456",
  "verify_note": "2026-11-26 复核：仍留待验证——与 2026-11-24 同批 4 条同一阻塞（抖音网页可播放、内容一致，但无下载途径、无法取得视频文件或直接播放地址，无法截取 GIF/关键帧）；本轮未重复尝试下载，待用户从手机抖音 App 保存视频文件后补验；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7678886080376098086",
  "verify_note": "2026-11-26 复核：仍留待验证——与 2026-11-24 同批 4 条同一阻塞（抖音网页可播放、内容一致，但无下载途径、无法取得视频文件或直接播放地址，无法截取 GIF/关键帧）；本轮未重复尝试下载，待用户从手机抖音 App 保存视频文件后补验；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7679648378807979305",
  "verify_note": "2026-11-26 复核：仍留待验证——与 2026-11-24 同批 4 条同一阻塞（抖音网页可播放、内容一致，但无下载途径、无法取得视频文件或直接播放地址，无法截取 GIF/关键帧）；本轮未重复尝试下载，待用户从手机抖音 App 保存视频文件后补验；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7687510825015315712",
  "verify_note": "2026-11-27 尝试验证：浏览器实测来源视频可正常播放（第15集 03:26），扇形展开/纵深叠排/圆柱环绕/球面排布/螺旋排布/波浪矩阵 6 种与提示词逐条一致；但抖音网页未提供下载途径（播放器无下载按钮、分享按钮点不开面板、右键被拦截、DOM 无 <video> 元素、页面无视频直链），无法取得视频文件截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7705257186435403058",
  "verify_note": "2026-11-27 尝试验证：浏览器实测来源视频可正常播放（第32集 01:52），点击范围/热区冲突/点击与拖动区分/点击反馈（按下变化、提交状态、失败提示）与提示词一致；“五查”第 5 项“链接”只在总结章（01:27）出现，未单独成章，提示词所列五查与总结章一致，无实质出入；但抖音网页未提供下载途径（同批 4 条页面结构相同，无下载按钮、无视频直链），无法取得视频文件截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7699718828174937379",
  "verify_note": "2026-11-27 尝试验证：浏览器实测来源视频可正常播放（第29集 01:21），卡片适合展示/列表适合查找/表格适合比数据（以“挑出宽度最大的图，用表格展示名称、尺寸、格式，同种数据上下对齐”为例）/切换布局保留搜索条件与勾选状态，与提示词逐条一致；但抖音网页未提供下载途径（同批 4 条页面结构相同，无下载按钮、无视频直链），无法取得视频文件截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7701961806482279715",
  "verify_note": "2026-11-27 尝试验证：浏览器实测来源视频可正常播放（第31集 01:04），选择器用于选择/菜单用于操作、选项少直展、选项多分组滚动、与 AI 沟通要点（选什么、选完做什么、结果留在哪）与提示词逐条一致；视频另有一节“输入框的使用”（00:42，熟悉信息可直接输入），提示词未列出，不冲突；但抖音网页未提供下载途径（同批 4 条页面结构相同，无下载按钮、无视频直链），无法取得视频文件截取 GIF/关键帧，故留待验证；不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7701274323436227880",
  "verify_note": "2026-11-28 备注：与 2026-11-24/11-27 各批同一阻塞（抖音网页无下载途径，无法取得视频文件截取 GIF/关键帧），本轮未重复尝试下载，留待验证；待用户从手机抖音 App 保存视频文件后补验，不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7707974421738278187",
  "verify_note": "2026-11-28 备注：与 2026-11-24/11-27 各批同一阻塞（抖音网页无下载途径，无法取得视频文件截取 GIF/关键帧），本轮未重复尝试下载，留待验证；待用户从手机抖音 App 保存视频文件后补验，不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7707970051038645546",
  "verify_note": "2026-11-28 备注：与 2026-11-24/11-27 各批同一阻塞（抖音网页无下载途径，无法取得视频文件截取 GIF/关键帧），本轮未重复尝试下载，留待验证；待用户从手机抖音 App 保存视频文件后补验，不许用生成图冒充。"
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
  "source_video": "https://www.douyin.com/video/7707976118627798312",
  "verify_note": "2026-11-28 备注：与 2026-11-24/11-27 各批同一阻塞（抖音网页无下载途径，无法取得视频文件截取 GIF/关键帧），本轮未重复尝试下载，留待验证；待用户从手机抖音 App 保存视频文件后补验，不许用生成图冒充。"
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

## 2026-11-18 · 公开渠道收集（第二轮：旅行/引导/智能家居/仪表盘可读性/播客）

来源：HitPaw《GPT Image 2 Prompts for UI Design》旅行与智能家居节、Lovable UI prompts（新手引导流程、空/加载状态）、Medium《Dashboard UI Design: 12 Real App Examples》（仪表盘可读性九项检查）、Design Lounge《Slow Archive podcast player》（章节波形播客播放器）、UXCharan《216 AI Prompts for UX/UI Designers》（新手引导文案）。以上均为搜索结果原文核对；提示词按主题原创改写，标注「同类收集，非原作摘录」，不冒充原作逐字摘录。已与正式库 29 条 + 待验证区去重：空/加载状态与正式库 detail-states-complete 同主题已跳过，深色渐变落地页与 landing-ai-product（深色科技渐变 variant）同风格已跳过。

## 2026-11-19 · 公开渠道收集（Visualizee.ai 游戏 UI / Carat 简历设计）

来源：Visualizee.ai《Game UI Design with AI: Interface Mockups Fast》（HUD、主菜单、背包三节）、Carat《Resume Design Prompts》（极简双栏、信息图简历两条）。以上均为已打开页面核对原文，提示词为原文摘录；库里此前没有游戏 UI 与简历/文档类条目，已与正式库 37 条 + 待验证区去重，无重复。

## 2026-11-19 · 公开渠道收集（登录页/日历/结账/个人主页）

来源核对：登录页见 Superdesign 登录页提示词库（搜索结果原文：社交登录优先、单密码框、单主按钮、找回链接、具体报错）；日历/日程与个人主页见 Techpresso《30 Claude Prompts That Design UI Screens》对应节（搜索结果原文）；结账见 Techpresso《30 Claude Prompts That Build Checkout Pages》购物车到支付节（搜索结果原文）。以上 4 条均为库里没有的页面类型（登录页、日历、结账、个人主页），只进待验证区；提示词按来源要点原创改写，标注「同类收集，非原作摘录」。




## 2026-11-19 · 公开渠道收集（第二轮：404/通知中心/搜索筛选/学习仪表盘/博客阅读/活动票务）

来源核对：404 错误页见 Medium《Top 10 Easy Prompts for Professional UI Design with designer-skill》（第 10 条，搜索结果原文）与 Liniqo《404 page and error page design》（AI 生成器提示词与插画尺寸要点，搜索结果原文）；通知中心见 design.dev《Toast Notification Stack》提示词模板（四种类型、自动消失进度条）与 JSBits《Design a Notification Center & Toast System》（Toast + 持久通知中心双面结构，搜索结果原文）；搜索筛选见 21st.dev《Filter Menu》与《Search Results》组件说明（分组筛选、可移除 chips、清空全部、键盘导航，搜索结果原文）；学习仪表盘见 danbyers.ai《Build a Learning Dashboard with AI》（顶部四张数据卡+课程/项目进度+深色主题，搜索结果原文）；博客阅读页见同一 Medium 文第 6 条博客主页提示词与 NotVibesCoded UI 提示词库博客类（单栏阅读视图、吸顶目录，搜索结果原文）；活动票务见 Ticko 票务 App 案例研究（发现→详情→选座→结账→票据流程、分区配色选座）与 Showpass 选座地图指南（按票种分区定价、最佳座位推荐，搜索结果原文）。以上 6 条均为库里没有的页面/功能类型，只进待验证区；提示词按来源要点原创改写，标注「同类收集，非原作摘录」，不冒充原作逐字摘录。已与正式库 41 条 + 待验证区 49 条去重：404 与 detail-states-complete（通用空/加载/错误态）不同，是带品牌插画与找回路径的整页；通知中心与 spt-overlay-six（浮层选型）不同，是持久通知列表+Toast 双面系统；学习仪表盘与 saas-dashboard-linear（通用 SaaS 仪表盘）不同，是课程进度/连胜/学习时长场景；博客阅读页与 landing-editorial（杂志风落地页）不同，是长文阅读页而非营销落地页；活动票务与 ecom-checkout-flow（购物车到支付）不同，是选座地图+票种分区流程。


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

## 2026-11-23 · 公开渠道收集（第二轮：停车找位/航班动态/用药提醒/商品详情页/语音助手/团队权限）

来源核对：停车找位见 Lovable Prompts 智能停车预约系统提示词（搜索/筛选/地图/预约/二维码通行）与 Pramod Mani《Smart Parking Solution》iPARK 案例（搜索结果原文核对）；航班动态见 webdevpuneet《Flight Status Tracker》卡片片段附带的“Prompt to recreate it”原文（航班号/航线/状态 pill/计划与实际时间/航站楼登机口座位、data-status 单一状态源，搜索结果原文核对）与 DesignCode 登机牌模块说明；用药提醒见 mejba.me《Claude/ChatGPT Prompt to Design a Medication Reminder App UI》全文模板（今日时间线/一键确认/余量追踪/照护者视图，搜索结果原文核对）；商品详情页见 aiwebstyle《Product Detail Page》配方（八段顺序、诚实占位规则，搜索结果原文核对）；语音助手见 mobileappdesign.io《Voice assistant UI: how 19 AI apps put a microphone on the chat screen》（19 款 App 三层语音结构，搜索结果原文核对）+ shadcn.io AI 语音助手块（四态 Idle/Listening/Thinking/Speaking、波形只在聆听/说话时动）+ Stream 语音代理视觉指南；团队权限见 justfigma《Team Roles & Permissions UI》与 Humbleteam《B2B SaaS roles and permissions UX》（成员列表/邀请流程/权限矩阵/自定义角色，搜索结果原文核对）。以上 6 条均为库里没有的场景（停车找位与 mobile-ride-hailing-night 打车场景不同；航班动态与 mobile-travel-booking 预订流程不同，是出行当天的状态与登机牌；用药提醒与 mobile-health 日常活动圆环不同，是按时服药管理；商品详情页与 ecom-checkout-flow 结账、ecom-ar-tryon-product 试穿不同，是购买决策页本身；语音助手与 ai-chat-app 文字对话不同，是语音四态界面；团队权限与 saas-settings-master-detail 设置页布局不同，是成员/角色/权限管理功能），提示词均按主题原创改写，标注「同类收集，非原作摘录」，只进待验证区。已与正式库 57 条 + 待验证区 73 条去重，无重复。

### 停车找位 App：地图找位+预约+扫码进出 (`mobile-parking-finder`)

```json
{
 "id": "mobile-parking-finder",
 "title": "停车找位 App：地图找位+预约+扫码进出",
 "category": "移动端App",
 "styles": [
  "停车",
  "地图",
  "出行"
 ],
 "scenario": "做停车找位/预约 App，希望开车时一眼看清最近最便宜的空位时",
 "prompt": "Design a mobile parking finder app: a map-first home screen showing nearby parking facilities as pins with live availability and price per hour, searchable and filterable by location, distance, price and availability; tapping a pin shows the facility card (spots left, rate, walking distance, open hours) and lets the driver reserve a slot for a date and time with no double bookings; after payment the driver gets a unique QR parking pass for entry and exit; a 'Find my car' view guides the driver back to the parked spot. Keep it driver-safe: minimal text, big touch targets, voice input for the vehicle, icons over words, and only the closest lots shown while driving. Light theme, one blue accent (#1978E5), Inter type, 8px radii, clean minimalist layout.",
 "prompt_zh": "停车找位 App：地图首页显示附近停车场空位与时价、可按位置距离价格筛选，点图钉看余量费率并预约时段，支付后得二维码通行证进出，另有「找回我的车」导航；驾驶场景下字少键大、可语音输入。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T09:15:00+08:00",
 "source": "Lovable Prompts 智能停车预约系统提示词 + Pramod Mani《Smart Parking Solution》iPARK 案例（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

### 航班动态/登机牌：状态卡片+登机牌 (`mobile-flight-status`)

```json
{
 "id": "mobile-flight-status",
 "title": "航班动态/登机牌：状态卡片+登机牌",
 "category": "移动端App",
 "styles": [
  "航班",
  "登机牌",
  "出行"
 ],
 "scenario": "做航班动态查询或登机牌界面，希望延误、登机口变化一眼可读时",
 "prompt": "Design a flight status tracker card plus a boarding pass: the status card shows the flight number, two airport codes with city names on either end of a route line with an inline SVG plane icon between two dots, and a status pill in the top-right (On Time / Delayed / Boarding / Departed). Below the route, departure and arrival times in two columns, each showing scheduled and actual time — the scheduled time gets a strikethrough and the actual time recolors when the flight is delayed. A meta row shows terminal, gate and seat; the gate value can change independently (reassigned when boarding starts). Drive all state from a single data-status attribute on the outer card so every color change keys off it. The boarding pass below is a clean card: passenger name, flight, gate, seat, date and times, a perforated dotted tear line and a scannable barcode strip. Dark-mode ready, high contrast, tabular numerals for times.",
 "prompt_zh": "航班动态卡+登机牌：航线两端机场代码与城市、飞机图标航线、右上状态 pill（准点/延误/登机/已出发），计划与实际时间并列（延误时计划时间划线、实际时间变色），航站楼/登机口/座位行可独立变更；下方登机牌带虚线撕口与条码，深色模式可用。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T09:15:00+08:00",
 "source": "webdevpuneet《Flight Status Tracker》片段附带的复现提示词原文 + DesignCode 登机牌模块说明（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

### 用药提醒 App：今日时间线+一键确认+余量追踪 (`mobile-medication-reminder`)

```json
{
 "id": "mobile-medication-reminder",
 "title": "用药提醒 App：今日时间线+一键确认+余量追踪",
 "category": "移动端App",
 "styles": [
  "用药提醒",
  "健康",
  "无障碍"
 ],
 "scenario": "做用药提醒/服药管理 App，用户多为长辈或需同时管多种药时",
 "prompt": "Design a medication reminder app for elderly patients and caregivers managing complex regimens: the home screen is today's schedule as a timeline, color-coded by time of day (morning / noon / evening / night), each dose showing a photo of the pill for visual identification plus name and dosage. One-tap confirmation: large Take / Skip / Snooze buttons (minimum 48px targets) with a satisfying confirmation animation and timestamp logging. Medication setup asks name, dosage, photo, schedule and refill count; a refill tracker counts pills remaining, warns when low and offers a pharmacy quick-call; an interaction checker warns when a new medication conflicts with existing ones. A caregiver view shares adherence reports and missed-dose alerts; history shows an adherence calendar (taken / missed / skipped) exportable as a PDF for doctor visits. Maximum clarity, minimum cognitive load: 18px+ body type, 24px+ headings, high contrast, no thin fonts, no complex setup wizards, no social or gamification features — this is medical, not a game.",
 "prompt_zh": "用药提醒 App：今日时间线按早中晚夜配色、药片照片识别，一键服药/跳过/稍后（≥48px 大按钮、带时间戳记录），余量倒数+药房快捷拨打、药物相互作用警告、照护者视图与可导出 PDF 的服药日历；大字高对比、无游戏化。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T09:15:00+08:00",
 "source": "mejba.me《Claude/ChatGPT Prompt to Design a Medication Reminder App UI》全文模板（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

### 电商商品详情页：图库+购买盒+信任条+评价 (`ecom-product-detail`)

```json
{
 "id": "ecom-product-detail",
 "title": "电商商品详情页：图库+购买盒+信任条+评价",
 "category": "电商零售",
 "styles": [
  "商品详情",
  "电商",
  "转化"
 ],
 "scenario": "做电商商品详情页，希望购买决策链路一屏讲清、不靠编造的好评撑场时",
 "prompt": "Build a product detail page for one physical product, in exactly this section order — the order is the argument: 1) Breadcrumb, three levels maximum, current page as text not a link. 2) Gallery: four images minimum, including one in use and one showing scale; never auto-advance — a carousel that moves while someone reads is a carousel they will misread; on desktop a sticky left column of stacked images with the buy box scrolling independently on the right, on mobile a horizontal swipe strip with visible dots. 3) Buy box: name, price with tax basis, variant control (size and colour — changing the variant changes the photograph too), quantity stepper, Add to cart, and a delivery date (name the date, not '3-5 business days'); all of it above the fold on a phone. 4) Trust strip, four items maximum, each answerable in one sentence: shipping cost, return window (30 days), warranty, payment methods. 5) Description that absorbs the doubts the buy box could not. 6) Reviews: a summary with a real count, then three reviews with dates — show the three-star review first; never invent a 4.8 average from thousands of reviews, use an honest placeholder instead. 7) Cross-sell. Mobile sticky buy bar past the main CTA fold; accessible custom selectors with visible focus and keyboard routes.",
 "prompt_zh": "商品详情页：面包屑→图库（≥4 张含使用与比例图、不自动轮播）→购买盒（名称/含税价/规格/数量/加购/具体送达日期，手机首屏可见）→信任条（运费/30 天退货/质保/支付方式最多四项）→描述→评价（真实数量、三星评价放第一，不编造高分）→关联推荐。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T09:15:00+08:00",
 "source": "aiwebstyle《Product Detail Page》配方（八段顺序与诚实占位规则，搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

### AI 语音助手：四态波形+实时转写 (`ai-voice-assistant`)

```json
{
 "id": "ai-voice-assistant",
 "title": "AI 语音助手：四态波形+实时转写",
 "category": "AI产品",
 "styles": [
  "语音助手",
  "波形",
  "对话"
 ],
 "scenario": "做 AI 语音对话界面，希望听着/想着/说着三种状态一眼分清时",
 "prompt": "Design an AI voice assistant screen: a large state word (Idle, Listening, Thinking, Speaking) beside a waveform that moves only while it is listening or the assistant is speaking aloud; a transcript log that fills word by word as speech is recognised, so mistakes can be caught and followed in noisy places. The microphone button lights up unmistakably while listening; Mute keeps the reply on screen but still; a speed control sets the speaking rate from 0.75x to 1.5x; an End session button sits in the same place as Start. Support barge-in: speaking while the assistant talks stops its audio immediately. Ask for microphone access only when the user taps the button, explain why first, and show how to allow it if denied; always keep a text input available as an alternative. The waveform is decorative and hidden from assistive technology — the state word and one polite status line carry the meaning; under reduced motion the waveform stops and each line appears whole. When the session ends, show a short summary of turns, length and words.",
 "prompt_zh": "AI 语音助手屏：Idle/Listening/Thinking/Speaking 四态大字+波形（只在聆听与说话时动）、实时逐词转写可纠错，麦克风按钮点亮态明显、可随时打断插话、支持静音与 0.75–1.5 倍语速；仅在点按时请求麦克风权限、始终保留文字输入，减动效时波形静止整行显示。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T09:15:00+08:00",
 "source": "mobileappdesign.io《Voice assistant UI: how 19 AI apps put a microphone on the chat screen》+ shadcn.io AI 语音助手块 + Stream 语音代理视觉指南（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

### SaaS 团队角色与权限：成员列表+邀请+权限矩阵 (`saas-team-roles`)

```json
{
 "id": "saas-team-roles",
 "title": "SaaS 团队角色与权限：成员列表+邀请+权限矩阵",
 "category": "SaaS后台",
 "styles": [
  "团队权限",
  "角色",
  "后台设置"
 ],
 "scenario": "做 B2B SaaS 的团队成员与权限管理，希望谁能干什么一目了然时",
 "prompt": "Design a B2B SaaS team roles and permissions area under Settings → Team: a member list where each row shows avatar (initials), name and email, a role badge (Owner / Admin / Member / Viewer / Billing), status (Active / Pending with 'Invited 3d ago' / Suspended) and last active, with actions Change role, Resend invite and Remove in an overflow menu. An invite flow in four steps — email(s), role picker with a one-line description per role (default Member), optional message, then a seat check ('Using 8 of 10 seats') that blocks or upsells at the limit. A permissions matrix as a live screen: one row per permission worded as a customer would say it ('Export customer data'), grouped by product area, one column per role with the number of people assigned; cell values in words — Allowed, Not allowed, Own items only, Assigned projects only — never colour alone. Offer custom roles (built on a default role, with grouped permission toggles and search) and preset templates (Billing Admin, Content Editor, Auditor) to duplicate; system roles are view-only. Gate destructive actions (remove member, change to Admin, transfer ownership) with confirmation and re-authentication; add a per-person view answering 'why can she do this?' and log every change to an audit log.",
 "prompt_zh": "团队角色与权限：成员列表（头像/姓名邮箱/角色徽章/待激活与上次活跃/操作菜单）+四步邀请（邮箱/带说明的角色选择/可选留言/席位占用检查）+权限矩阵（按产品区分组、单元格用文字而非仅颜色）+自定义角色与预设模板，危险操作需确认与二次验证并记审计日志。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-23T09:15:00+08:00",
 "source": "justfigma《Team Roles & Permissions UI in Figma》+ Humbleteam《B2B SaaS roles and permissions UX: a design guide》（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-23）"
}
```

## 2026-11-24 · 公开渠道收集（协作文档/电子签名/餐厅扫码点单/表单构建器/播客后期）

来源核对：5 条原文均已打开核对、提示词按要点原创改写（同类收集，非原作摘录）；与正式库 57 条 + 待验证区 79 条逐一去重，无重复（协作文档编辑器与三栏收件箱/数据表格场景不同；电子签名与简历模板场景不同，是签署流程本身；餐厅扫码点单与外卖点餐场景不同，是到店扫码+同桌合单+分账；表单构建器与数据表格/设置页场景不同，是拖拽搭建表单；播客后期制作与播客播放器场景不同，是录音剪辑/去填充词/响度归一/出片流程）。added_at 统一记本轮时间 2026-11-24T08:10:00+08:00。

### 协作文档编辑器：工作区/文件夹/富文本+实时协作 (`saas-doc-editor-collab`)

```json
{
  "id": "saas-doc-editor-collab",
  "title": "协作文档编辑器：工作区/文件夹/富文本+实时协作",
  "category": "SaaS后台",
  "styles": [
    "极简",
    "协作",
    "文档"
  ],
  "scenario": "10 人小团队的协作文档/知识库，Notion 风格",
  "prompt": "Design a collaborative document editor for a 10-person team, clean and minimal like Notion: workspaces containing folders containing pages, shown as a collapsible sidebar tree; a rich text editor with H1/H2/H3 headings, bullet and numbered lists, bold, italic, code blocks and blockquotes, plus a slash-command menu and floating format toolbar; live cursors and presence avatars when teammates edit the same page; search across all pages by title and content; page sharing set to private (team only) or public link; each page shows last-edited timestamp and editor name. White background, soft gray text, one restrained accent color, generous whitespace.",
  "prompt_zh": "协作文档编辑器：工作区→文件夹→页面的侧边树+富文本（标题/列表/代码块/引用）+斜杠菜单+实时光标与在线头像，全文搜索、私有/公开链接分享，Notion 式极简。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T08:10:00+08:00",
  "source": "Blink《How to Build a Document Editor with AI (Notion Alternative in a Weekend)》全文提示词核对改写（工作区/文件夹/页面层级、富文本、搜索、分享、侧边导航、最后编辑信息，2026-11-24）；https://blink.new/blog/how-to-build-document-editor"
}
```

### 电子签名工具：上传 PDF 拖字段发签署 (`saas-esignature-send-sign`)

```json
{
  "id": "saas-esignature-send-sign",
  "title": "电子签名工具：上传 PDF 拖字段发签署",
  "category": "SaaS后台",
  "styles": [
    "极简",
    "效率",
    "商务"
  ],
  "scenario": "自由职业者/小团队每月发少量合同的轻量签署工具",
  "prompt": "Design a lightweight e-signature tool for freelancers who send a handful of contracts each month: a calm dashboard with one bold 'New Contract' button; after uploading a PDF, drag signature, date and text fields onto the document preview with snapping guides; below the preview, a signer list showing each signer's email and a status pill (Sent, Viewed, Signed); a signing view for recipients that is stripped down to the contract preview, highlighted fields and one big button to sign by typing or drawing. Notion/Linear-inspired style: white space, soft grays, clean typography, subtle shadows, rounded buttons; big tap targets on mobile. Every step should feel obvious and stress-free.",
  "prompt_zh": "轻量电子签名：上传 PDF 后拖签名/日期字段到预览上，签署人列表带已发送/已查看/已签署状态；对方签署页只留合同预览+高亮字段+一个大签署按钮，Notion/Linear 式冷静清晰。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T08:10:00+08:00",
  "source": "ProvenStartups《DocuSign Forgot the Freelancers》UI Prompt 原文核对改写（New Contract、拖字段、签署人状态列表、极简签署页，2026-11-24）；https://provenstartups.substack.com/p/docusign-forgot-the-freelancers"
}
```

### 餐厅扫码点单：桌码认桌+合单+分账 (`ecom-restaurant-qr-order`)

```json
{
  "id": "ecom-restaurant-qr-order",
  "title": "餐厅扫码点单：桌码认桌+合单+分账",
  "category": "电商零售",
  "styles": [
    "移动端",
    "点餐",
    "暖色"
  ],
  "scenario": "早午餐店/餐厅到店扫码点单，18 张桌",
  "prompt": "Design a mobile table QR ordering flow for an 18-table brunch cafe: guests scan the QR code on their table, the screen confirms the table number first, then shows the menu in sticky category tabs with dish photos, prices, allergen tags and a sold-out state that greys dishes out; each dish has modifiers (size, spice level, extra toppings, remove an ingredient); orders go to one shared table tab so guests can keep adding items in waves, and the kitchen sees each order with its table number; at the end guests split the bill and pay from their phones. Soft yellow and white design, big tap targets for one-handed use, prices right-aligned in one consistent format.",
  "prompt_zh": "餐厅扫码点单：扫桌码先确认桌号，分类菜单+菜品图/过敏原标签/售罄置灰，配菜选项齐全；同一桌共用一个合单、厨房按桌号出票，最后分账付款，淡黄暖色、大触控目标。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T08:10:00+08:00",
  "source": "Gappsy《Restaurant Ordering App Prompts》第 4 条 Table QR ordering 原文核对改写（桌码认桌、合单、分账、淡黄配色，2026-11-24）；https://www.gappsy.com/prompts/restaurant-ordering-app/"
}
```

### 在线表单构建器：拖拽字段+条件逻辑 (`saas-form-builder`)

```json
{
  "id": "saas-form-builder",
  "title": "在线表单构建器：拖拽字段+条件逻辑",
  "category": "SaaS后台",
  "styles": [
    "效率",
    "拖拽",
    "模块化"
  ],
  "scenario": "个人/小团队用的类 JotForm 表单搭建工具",
  "prompt": "Design a personal form builder app that rivals JotForm: a three-column workspace — left sidebar with draggable field types (text input, textarea, checkbox, radio, dropdown, date, file upload, rating), center canvas where fields are dropped, reordered and resized, right properties panel for label, placeholder, required and validation rules; templates gallery to start from; conditional logic that shows or hides fields based on earlier answers; live preview toggle (desktop/mobile) and a responses view with a simple table; local-first storage with clear privacy wording. Modern, modular design: clean neutrals, one accent color, clear drag handles and drop indicators, fully responsive and keyboard-accessible.",
  "prompt_zh": "表单构建器：左侧字段库拖拽到中间画布、右侧属性面板改校验与必填，模板库起步、按答案显示/隐藏字段的条件逻辑，实时预览+回收数据表，本地优先、隐私明确。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T08:10:00+08:00",
  "source": "Kaushik Sarkar《Personal Form Builder App Design: Drag-and-Drop Editor》（转引 prompts.chat 全文提示词）核对改写（拖拽编辑器、模板、条件逻辑、隐私，2026-11-24）；https://www.kaushiksarkar.com/blog/personal-form-builder-app-design-drag-and-drop-editor-with-conditional-logic-mas"
}
```

### 播客后期制作：录音进、成片出（波形剪口+章节+示范文案） (`content-podcast-postproduction`)

```json
{
  "id": "content-podcast-postproduction",
  "title": "播客后期制作：录音进、成片出（波形剪口+章节+示范文案）",
  "category": "内容社交",
  "styles": [
    "深色",
    "音频",
    "工作室"
  ],
  "scenario": "独立播客主每周一期的后期制作：去填充词、响度归一、出成片资料包",
  "prompt": "Design PodcastPilot, an audio production app for indie podcasters — audio production, not a video editor: upload a raw recording and get a cleaned master plus a publish kit. Episode page centers on a dark studio waveform with cut markers for detected filler words and silences over 1.2 seconds, a bulk 'Accept fillers' button, per-cut accept/reject, and loudness normalization to the show target; the right panel holds the publish kit — show notes, 8-12 chapters, 3 title options and 5 pull quotes, with a Regenerate notes button that does not re-run the audio; episode status flows upload → processing → review → published. Dark studio background, off-white text, one lime accent, mono type for timestamps, Geist-style clean interface.",
  "prompt_zh": "播客后期制作：上传原始录音，波形上标出填充词/静音剪口可批量接受，响度归一出成片；右侧出 show notes、8-12 章节、3 个标题、5 条金句，深色录音棚风+青柠强调色。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T08:10:00+08:00",
  "source": "Weekend MVP《Raw recording to polished episode — PodcastPilot》AI Prompts to Build This（项目搭建/核心功能两节）核对改写（波形剪口、填充词检测、响度归一、章节与示范文案，2026-11-24）；https://www.weekendmvp.app/ideas/ai-podcast-producer"
}
```

## 2026-11-24 · 公开渠道收集（AI With Ghost / Lovable Prompts）

来源：两页原文均已打开核对，按统一格式改写，非逐字摘录；与正式库 61 条及待验证区去重（避开已有空状态/骨架屏、设置页、数据看板、登录页、AI 聊天等同场景条目）。本批 5 条先进待验证区，验证通过才进正式库。

### 开发者工具落地页：Identity/Structure/Content/Motion/Never 五段式简报 (`landing-devtool-tracebit-brief`)

```json
{
  "id": "landing-devtool-tracebit-brief",
  "title": "开发者工具落地页：Identity/Structure/Content/Motion/Never 五段式简报",
  "category": "落地页官网",
  "styles": [
    "深色",
    "开发者工具",
    "克制"
  ],
  "scenario": "面向后端开发者的日志搜索工具单页落地页（以 Tracebit 为示例产品）",
  "prompt": "Build a single-page landing page for \"Tracebit\", a log search tool for backend developers. Stack: React + Tailwind CSS, one file, responsive down to 360px. IDENTITY: background #0A0A0B, text near-white at 92%, secondary text at 60%; one accent only, #FF5A1F, used for the primary CTA, one highlight per section and focus rings; font Inter, weights 400 and 600 only, JetBrains Mono for code; radius 12px; borders 1px white at 8% opacity. STRUCTURE: (1) sticky nav, wordmark left, 3 links plus accent Start free button right, adds backdrop blur and bottom border after 24px scroll; (2) left-aligned hero, headline clamp(2.75rem, 6vw, 4.75rem), tracking -0.03em, max 8 words, subline max-width 34rem at 60% opacity, primary plus ghost CTA, right side a terminal window showing 6 lines of a log query with one matched line highlighted in the accent; (3) logo row of 6 grey placeholder wordmarks at 40% opacity; (4) features as 3 rows alternating text and visual sides, each visual a bordered panel with a faint 24px grid background; (5) one large testimonial quote in display type with placeholder name clearly marked [CUSTOMER NAME]; (6) pricing with 3 tiers, middle tier elevated with accent border and Most popular tag; (7) FAQ accordion, one item open at a time, 5 questions; (8) final CTA band, then a minimal 2-row footer. CONTENT RULES: use the placeholder copy in [BRACKETS] where real content is needed; do not invent customer names, logos, numbers or reviews. MOTION: sections fade up 16px over 500ms on first entry into view, children stagger 60ms; cards lift 3px on hover; respect prefers-reduced-motion. NEVER: no gradient text, no emoji in headings, no three-icon feature row, no stock illustrations, no carousel, no more than one accent colour, no centred hero.",
  "prompt_zh": "开发者工具落地页按 Identity/结构/文案规则/动效/Never 五段写简报：深底单强调色、左对齐大标题配终端窗口、交替特性行与三档定价，结尾用禁令兜底不跑偏成通用模板页。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T09:20:00+08:00",
  "source": "AI With Ghost《How to Prompt Any AI Builder for a Landing Page That Doesn't Look AI-Generated》Tracebit 全文示例提示词核对改写（五段式结构、#0A0A0B/#FF5A1F、Inter 400/600、终端窗口、NEVER 禁令，2026-11-24）；https://aiwithghost.com/news/news-how-to-prompt-any-ai-builder-for-a-landing-page-that-doesnt-look-ai-generated-fu/"
}
```

### 弹窗与对话框系统：三种尺寸底座+确认框+移动端底部抽屉 (`saas-modal-dialog-system`)

```json
{
  "id": "saas-modal-dialog-system",
  "title": "弹窗与对话框系统：三种尺寸底座+确认框+移动端底部抽屉",
  "category": "SaaS后台",
  "styles": [
    "系统化",
    "弹窗",
    "无障碍"
  ],
  "scenario": "已有应用里第一次出现确认、编辑或删除弹窗之前，先统一弹窗系统",
  "prompt": "Design one modal and dialog system for the whole app, before the first confirm, edit or delete dialog is built: a base modal in 3 sizes (small, medium, large) with a shared header, body and footer layout, plus a confirm dialog variant with a clear destructive action; shared rules for focus trapping, Escape to dismiss, click-outside behaviour, and what happens to unsaved input when the dialog closes; on mobile the same dialogs become bottom sheets. Every dialog states its purpose in the title, keeps one primary action, and returns focus to the element that opened it. Clean, calm style: neutral surfaces, one accent colour, 12px radius, subtle shadow, generous padding; no decorative illustration inside dialogs.",
  "prompt_zh": "全应用只用一套弹窗系统：三种尺寸底座+确认框变体，统一焦点、关闭与未保存输入规则，移动端变底部抽屉，标题说清目的、只留一个主操作。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T09:20:00+08:00",
  "source": "Lovable Prompts《Lovable UI prompts: 14 for screens, empty states and dashboards》Modal & Dialog Component System 卡片核对改写（三种尺寸底座、确认框、焦点/关闭/未保存规则、移动端底部抽屉，2026-11-24）；https://Lovable-prompts.com/prompts/ui-ux"
}
```

### 响应式导航栏：单配置模块+768px 以下抽屉+键盘无障碍 (`saas-responsive-navbar`)

```json
{
  "id": "saas-responsive-navbar",
  "title": "响应式导航栏：单配置模块+768px 以下抽屉+键盘无障碍",
  "category": "SaaS后台",
  "styles": [
    "导航",
    "响应式",
    "无障碍"
  ],
  "scenario": "新项目先搭的页面框架：服务端渲染导航，之后所有功能页继承它",
  "prompt": "Build a responsive navbar for a web app from one config module, as the first piece of the app shell before any feature screen: desktop shows the logo left, navigation links centre and user actions right, with the active page shown by underline and heavier weight; below 768px it becomes a mobile Sheet drawer with the same links and actions; the navbar is server-rendered, sticky, and fully keyboard and screen-reader accessible with visible focus states and proper aria labels. Clean minimal style: neutral background, one accent colour, 8px spacing grid, 48px bar height on desktop; no hamburger on desktop, no duplicated navigation in the footer.",
  "prompt_zh": "先搭响应式导航再做功能页：单配置模块驱动桌面导航与 768px 以下抽屉，当前页以下划线+加粗标示，全键盘与读屏无障碍。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T09:20:00+08:00",
  "source": "Lovable Prompts《Lovable UI prompts: 14 for screens, empty states and dashboards》Responsive Navbar Builder 卡片核对改写（单配置模块、768px 以下 Sheet、当前态下划线+加粗、键盘与读屏支持，2026-11-24）；https://Lovable-prompts.com/prompts/ui-ux"
}
```

### 文件上传+打标签：拖拽上传、五种文件状态、可检索标签库 (`saas-file-upload-tagging`)

```json
{
  "id": "saas-file-upload-tagging",
  "title": "文件上传+打标签：拖拽上传、五种文件状态、可检索标签库",
  "category": "SaaS后台",
  "styles": [
    "文件",
    "拖拽",
    "标签"
  ],
  "scenario": "用户把自己的文件带进应用的个人资料库/素材库",
  "prompt": "Design a file upload and tagging UI for a personal library: drag-and-drop uploads into a private per-user bucket, with five named file states shown clearly — queued, uploading with progress, processing, ready, and failed with a retry action; server-side checks for file type and size with plain-language error messages; after upload, files get normalised tags from a shared tag list so the library can be filtered by tag, type and date; a list view shows thumbnail, name, size, upload date and tags, with search across file names and tags. Clean, calm style: neutral surfaces, one accent colour, clear drop zone with a dashed border, generous spacing; no fake sample files.",
  "prompt_zh": "文件上传加标签：拖拽进个人私有空间，五种状态（排队/上传中/处理中/就绪/失败可重试）一目了然，服务端校验类型大小，统一标签库供筛选检索。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T09:20:00+08:00",
  "source": "Lovable Prompts《Lovable UI prompts: 14 for screens, empty states and dashboards》File Upload + Tagging UI 卡片核对改写（拖拽上传、私有空间、五种文件状态、服务端类型大小校验、规范化标签筛选，2026-11-24）；https://Lovable-prompts.com/prompts/ui-ux"
}
```

### SEO 元标签编辑器：导入站点地图+实时搜索结果预览+重复标记 (`saas-seo-meta-editor`)

```json
{
  "id": "saas-seo-meta-editor",
  "title": "SEO 元标签编辑器：导入站点地图+实时搜索结果预览+重复标记",
  "category": "SaaS后台",
  "styles": [
    "SEO",
    "编辑器",
    "效率"
  ],
  "scenario": "上线前给待发布页面写标题与描述的内部工具",
  "prompt": "Design an internal SEO meta tag editor for page titles and meta descriptions: import pages from a sitemap, edit title and description per page with live character and pixel-width clipping shown against a realistic search-result preview; flag duplicate titles and descriptions across pages, warn when a title is too long or too short, and keep a revision history per page so earlier versions can be restored; export the finished set as CSV or JSON. Clean, efficient style: two-column layout with the page list left and the editor plus live preview right, neutral surfaces, one accent colour, mono type for pixel counts, clear save state; no invented rankings or traffic numbers.",
  "prompt_zh": "SEO 元标签内部编辑器：导入站点地图逐页改标题描述，实时搜索结果预览+像素宽度截断提示，重复标题标记、可回滚修订历史，导出 CSV/JSON。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-24T09:20:00+08:00",
  "source": "Lovable Prompts《Lovable UI prompts: 14 for screens, empty states and dashboards》SEO Meta Tag Generator UI 卡片核对改写（站点地图导入、实时搜索结果预览、像素宽度截断、重复标记、修订历史、CSV/JSON 导出，2026-11-24）；https://Lovable-prompts.com/prompts/ui-ux"
}
```

## 2026-11-25 · 公开渠道收集（Lovable Prompts / VibeFather / DocsBot / Taskade / Vibecode）

来源：五页原文均已打开核对，按统一格式改写，非逐字摘录；与正式库 65 条及待验证区去重（客服工单、婚礼邀请、儿童早教、面试安排、学生规划均为库里没有的新场景；学生规划与待验证区单日程/单番茄钟条目场景不同，已在来源行注明）。本批 5 条先进待验证区，验证通过才进正式库。

### 客服工单系统：表单+邮件进线、四态流转、一键认领 (`saas-support-ticketing`)

```json
{
 "id": "saas-support-ticketing",
 "title": "客服工单系统：表单+邮件进线、四态流转、一键认领",
 "category": "SaaS后台",
 "styles": [
  "客服",
  "工单",
  "系统化"
 ],
 "scenario": "2-15 人客服团队处理来自表单与邮件的客户请求，需要每单有人负责、不丢失时",
 "prompt": "Build a customer support ticketing tool for a team of 2 to 15 agents. Intake: requests arrive from a web form and a forwarded email address and become tickets with a status and an owner — no request gets lost between agents. Lifecycle: new, open, waiting on customer, resolved; replying changes status automatically and waiting on customer pauses the response clock; replying to a resolved ticket reopens it. Assignment: one owner per ticket, an unassigned queue visible to all, one-click Claim. Replies and internal notes: replies email the requester; internal notes render in a separate yellow block and can never be sent to the requester. Metrics: first-response and resolution time per agent and overall, with a soft target per priority highlighted on breach. Clean, calm style: neutral surfaces, one accent colour, clear status chips, generous spacing; the ticket list, the ticket detail with its reply thread, and the metrics view must all read from the same ticket records.",
 "prompt_zh": "客服工单系统：表单与邮件进线自动成单、新建/处理中/等客户/已解决四态流转、一单一人+待认领队列一键认领、内部备注黄色块永不外发、首响与解决时长按优先级设目标并标出超期。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-25T08:15:00+08:00",
 "source": "Lovable Prompts《Lovable App Builder Prompts: 30 Full Apps and the Best Practices》Customer Support Ticketing Tool 卡片核对改写（表单+邮件进线、四态流转、一键认领、内部备注不外发、首响/解决时长指标，2026-11-25）；https://Lovable-prompts.com/prompts/app-builder"
}
```

### 婚礼邀请与 RSVP 单页：象牙底+衬线名+倒计时+四章故事 (`landing-wedding-rsvp`)

```json
{
 "id": "landing-wedding-rsvp",
 "title": "婚礼邀请与 RSVP 单页：象牙底+衬线名+倒计时+四章故事",
 "category": "落地页官网",
 "styles": [
  "婚礼",
  "邀请",
  "优雅衬线"
 ],
 "scenario": "做婚礼邀请单页：宾客从群聊点开链接，三分钟内知道时间地点并完成 RSVP 时",
 "prompt": "Build a single-page wedding invitation and RSVP website. Hero: the couple's names in an elegant serif over an ivory background with a live countdown to the wedding date. Sections: a four-chapter love story, the schedule of the day as a vertical timeline, travel and stay notes for guests, an RSVP form (attending, party size, meal choice, dietary notes, one song request) that saves a thank-you card in the browser with a change-your-answer link, a guest FAQ, and registry placeholder cards. Palette: ivory and warm paper with sage and deep olive accents and one blush tone for hearts and highlights; Gilda Display for names and headings, Jost for body. All copy lives in one content file so the couple, venue, city and date can be swapped without touching layout. Mobile-first: most guests open the link from a group chat on a phone; within ten seconds a visitor knows who, where and when, and within two minutes they have answered the RSVP. Warm, personal, lightly funny tone; short paragraphs with concrete details (times, walking minutes, menu names).",
 "prompt_zh": "婚礼邀请单页：象牙底+优雅衬线大名+实时倒计时、四章爱情故事、当日流程竖时间线、交通住宿、RSVP 表单（出席/人数/餐食/忌口/点歌）本地保存感谢卡可改答案、FAQ 与礼单占位卡，文案集中一处可换新人场地日期。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-25T08:15:00+08:00",
 "source": "VibeFather《Wedding Invitation and RSVP Website》模板全文核对改写（象牙底、Gilda Display 衬线、倒计时、四章故事、竖时间线、RSVP 本地保存感谢卡，2026-11-25）；https://vibefather.ai/templates/wedding-invitation-and-rsvp-website"
}
```

### 儿童早教学习 App：拼音/数学/阅读游戏+星球按钮+家长面板 (`mobile-kids-learning`)

```json
{
 "id": "mobile-kids-learning",
 "title": "儿童早教学习 App：拼音/数学/阅读游戏+星球按钮+家长面板",
 "category": "移动端App",
 "styles": [
  "儿童早教",
  "游戏化",
  "太空"
 ],
 "scenario": "给 7-11 岁孩子做拼音、数学、拼写、阅读练习 App，学起来像游戏、家长能看进度时",
 "prompt": "Design a fun, colorful, mobile-first kids learning app for ages 7-11, covering math, phonics, spelling, writing and reading comprehension, where learning feels like a game. Home screen: a playful mascot squad in a space setting with four big star-shaped subject buttons. Grade selector: four planet-shaped buttons for grades 2 to 5 leading to rocket-shaped subject buttons. Practice screens: math missions with space-themed quizzes (e.g. count-the-planets multiplication), phonics quizzes with read-aloud pronunciation, spelling games, sentence building and reading logs. Progress: a space travel-log calendar and a mastery galaxy chart; badges unlock rewards. Parent dashboard (password-protected) shows the same progress. Visual system: bright blue main colour with pink, sunshine yellow and grass green accents on a light lavender starry background; rounded playful fonts; every touch target big enough for small fingers; cheerful sound feedback for correct and wrong answers. Use only original mascot characters, no copyrighted characters.",
 "prompt_zh": "儿童早教 App：7-11 岁数学/拼音/拼写/阅读游戏化练习，星形科目键+星球年级键+火箭科目键、太空旅行日志与掌握星系进度、徽章奖励、密码保护家长面板，大按钮+圆润字体+亮蓝粉黄绿配色。",
 "tools": [
  "v0",
  "Lovable",
  "即梦"
 ],
 "added_at": "2026-11-25T08:15:00+08:00",
 "source": "DocsBot《Stitch-Inspired Kids Learning Website》全文提示词核对改写（原提示词为 Stitch 风格灵感、明确不使用迪士尼原角色，本条按通用太空小伙伴形象改写；星形/星球/火箭按钮、拼音发音、家长面板，2026-11-25）；https://docsbot.ai/prompts/education/stitch-inspired-kids-learning-website"
}
```

### 面试安排：候选人选时段锁定+确认+面试官简报+评分卡 (`saas-interview-scheduling`)

```json
{
 "id": "saas-interview-scheduling",
 "title": "面试安排：候选人选时段锁定+确认+面试官简报+评分卡",
 "category": "SaaS后台",
 "styles": [
  "招聘",
  "日程",
  "自动化"
 ],
 "scenario": "招聘协调员不用邮件来回约面试：给候选人几个面试官已确认的时段、选定即锁定并自动通知时",
 "prompt": "Build an interview scheduling app. For each candidate and stage, offer a short list of times the interview panel has confirmed they can make, let the candidate pick one, and lock that slot while releasing the others. Send confirmations with the meeting link to the candidate and the panel; email each interviewer their brief (the candidate's CV and the stage-specific questions) the evening before, and prompt them for a scorecard an hour after the interview. Views: a board moving candidates through Slots Offered, Confirmed, Interviewed, Decided; a calendar of every confirmed interview across all open roles; a table of stage, panel, slot and scorecard status side by side. Automations: choosing a slot confirms to all parties and creates calendar entries; a candidate who has not chosen within 48 hours gets a nudge; a 'none of these work' option returns their constraints instead of starting an email thread. Clean, professional style: neutral surfaces, one accent colour, clear status chips, readable tables; every record carries its role, stage, panel and time zone.",
 "prompt_zh": "面试安排：每位候选人每轮只给面试官已确认的几个时段、选定即锁定其余释放、自动发确认与会议链接、前一晚发面试官简报（简历+本轮问题）、面后一小时催评分卡，看板/日历/表格三视图，48 小时未选自动提醒。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-25T08:15:00+08:00",
 "source": "Taskade《Interview Slot Scheduling Prompt for 2026》全文核对改写（候选人选时段锁定、自动确认、面试官简报、面后评分卡、看板/日历/表格三视图，2026-11-25）；https://www.taskade.com/prompts/booking-and-scheduling/interview-slot-confirmation-scheduler"
}
```

### 学生课表规划 App：今日课程+周课表+作业考试+番茄钟+成绩 (`mobile-student-planner`)

```json
{
 "id": "mobile-student-planner",
 "title": "学生课表规划 App：今日课程+周课表+作业考试+番茄钟+成绩",
 "category": "移动端App",
 "styles": [
  "学生规划",
  "课表",
  "学习"
 ],
 "scenario": "给中学生做课表+作业+考试+专注+成绩一体化的学习规划 App 时",
 "prompt": "Design a student planner app for high-school students. Home: a greeting with the student's name and date, pill chips switching between Classes, Exams and Tasks Due, today's classes as photo cards with subject in coloured condensed caps, topic, time and an Up Next / Tasks Due pill, plus a tickable daily study plan with a progress bar. Calendar: a day timeline (hour grid with a now-line), a month grid, and a Monday-Friday timetable of solid coloured blocks. Activities: tasks grouped Overdue / Today / Tomorrow / This Week / Later with a progress line and subtasks, exams with countdowns and scores, clubs and events. Focus: a dark screen with a glowing ring timer (focus and break modes) that logs sessions. Profile: stats tiles, a weekly focus bar chart, subjects with letter grades and a grade calculator. An AI study coach reads the planner and proposes study blocks on the calendar. Visual system: light pale-blue UI with white cards, brand blue #1E5BFF, bright cyan #1CE3F0 for selected chips and progress, navy #14197A headings; subject names in heavy condensed caps in the subject's colour.",
 "prompt_zh": "学生规划 App：首页今日课程照片卡+待办药丸+可勾选学习计划、日历（日时间线/月视图/周一至周五课表）、作业按截止分组+考试倒计时与分数、深色番茄钟、成绩计算器、AI 学习教练排学习块，浅蓝底+品牌蓝+亮青。",
 "tools": [
  "v0",
  "Lovable",
  "Cursor"
 ],
 "added_at": "2026-11-25T08:15:00+08:00",
 "source": "Vibecode《MyStudyLife Clone: Student planner App Template》全文提示词核对改写（今日课程卡、周课表、作业分组、考试倒计时、番茄钟、成绩计算器、AI 教练，2026-11-25）；https://www.vibecodeapp.com/templates/mystudylife — 与待验证区 mobile-calendar-schedule（单日程）、mobile-pomodoro-timer（单番茄钟）不同，本条为课表+作业+考试+专注+成绩一体化学生规划 App"
}
```

## 2026-11-25 · 公开渠道收集（直播电商/医生预约/投资组合/外卖追踪/心情日记）

来源核对：直播电商见 Vibefather《Live Shopping Stream Page》模板简报与 GPT Image Hub 直播间 UI 提示词（搜索结果原文）；医生预约见 GenDesigns《The Ultimate AI Design Prompt Library》第 90 条（搜索结果原文）；投资组合见 Design Lounge《Portfolio dashboard》构建简报（搜索结果原文）；外卖追踪见 Design Lounge《Phone order tracking》构建简报（搜索结果原文）；心情日记见 Mejba《Claude Prompt to Design a Mood & Diary Journal App Interface》（搜索结果原文）。以上 5 条均为库里没有的场景（直播带货、医生挂号、投资组合仪表盘、外卖订单追踪、私密心情日记），只进待验证区；提示词按来源要点原创改写，标注「同类收集，非原作摘录」，不冒充原作逐字摘录。已与正式库 65 条 + 待验证区去重：医生预约与 mobile-health（运动记录/健康数据）不同，是选科室-医生-时段的挂号流程；外卖追踪与 mobile-food（点餐首页）不同，是下单后的地图+ETA 追踪屏；投资组合与 mobile-fintech（钱包/记账首页）及 banking-web（银行门户）不同，是持仓/配置/调仓的券商仪表盘；心情日记与 mobile-meditation-app（冥想）不同，是情绪记录+日历+趋势洞察。

### 直播电商：主播画面+商品卡+聊天同屏 (`ecom-live-shopping-stream`)

```json
{
  "id": "ecom-live-shopping-stream",
  "title": "直播电商：主播画面+商品卡+聊天同屏",
  "category": "电商零售",
  "styles": [
    "直播电商",
    "直播间",
    "带货"
  ],
  "scenario": "做直播带货/直播购物界面，需要主播画面+商品卡+聊天同屏时",
  "prompt": "Design a mobile live-shopping stream interface (9:16): a full-bleed host video stage with the host presenting the product; top bar with host avatar, name, follower count, a Follow button, live viewer count and a ranking badge; floating gift hearts and a red-envelope countdown chip; a scrolling chat column bottom-left with short viewer messages and purchase alerts ('user_6789 just bought'); two stacked product cards bottom-right — the featured product with a 'Now presenting' badge, price, discount and Buy button, plus a secondary product; a bottom input bar ('Say something…') with emoji, cart, gift, share and more icons. Keep text legible over video with scrim gradients, make the Buy action thumb-reachable, and keep chat from covering the product cards.",
  "prompt_zh": "直播带货界面：全屏主播画面+顶栏主播信息与观看人数、礼物红包浮层、左下滚动聊天与下单提醒、右下双商品卡（正在讲解+次推）、底部输入栏与购物车，文字用渐变罩保证可读、购买按钮在拇指区。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-25T09:30:00+08:00",
  "source": "Vibefather《Live Shopping Stream Page》模板简报 + GPT Image Hub 直播间 UI 提示词（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-25）；https://vibefather.ai/templates/live-shopping-stream-page 与 https://www.gptimagehub.com/library/e-commerce-livestream-shopping-ui-mockup"
}
```

### 医生预约挂号：选科室+医生卡+7 天时段网格 (`mobile-doctor-appointment`)

```json
{
  "id": "mobile-doctor-appointment",
  "title": "医生预约挂号：选科室+医生卡+7 天时段网格",
  "category": "移动端App",
  "styles": [
    "医疗",
    "预约",
    "挂号"
  ],
  "scenario": "做医生预约/挂号 App，需要选科室、医生、日期时段时",
  "prompt": "Design an iOS doctor appointment booking app: a specialty dropdown at the top, then a doctor list of cards — photo, name, specialty, star rating and next available time. Tapping a doctor opens a booking sheet: a 7-day calendar strip, a time-slot grid where available slots are tinted and booked ones are gray, and a summary line of the selected doctor, date and time. One primary 'Book Appointment' button, an insurance note below it, and a confirmation state with Add to calendar. Professional blue and white palette, large tap targets, clear empty-day handling when no slots are free.",
  "prompt_zh": "医生预约 App：顶部选科室、医生卡（照片/姓名/科室/评分/最近可约时间）、7 天日历条+时段网格（可约着色、已约置灰）、选中汇总行+预约主按钮与保险提示、确认态可加入日历，专业蓝白、大点击区。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-25T09:30:00+08:00",
  "source": "GenDesigns《The Ultimate AI Design Prompt Library: 100+ Copy-Paste Prompts for Mobile & Web UI (2026)》第 90 条医生预约提示词（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-25）；https://gendesigns.ai/blog/ai-design-prompt-library-100-prompts"
}
```

### 投资组合仪表盘：总资产+可 scrub 走势+配置环+调仓卡 (`fin-portfolio-dashboard`)

```json
{
  "id": "fin-portfolio-dashboard",
  "title": "投资组合仪表盘：总资产+可 scrub 走势+配置环+调仓卡",
  "category": "金融",
  "styles": [
    "投资组合",
    "仪表盘",
    "深色"
  ],
  "scenario": "做券商/基金投资组合仪表盘，需要总资产、走势、持仓与调仓时",
  "prompt": "Design a calm investment portfolio dashboard for a brokerage account: a 64px serif total portfolio value at the top, range tabs (1D, 1W, 1M, 3M, YTD, 1Y, ALL) over a scrubbable value chart with a hover readout of date, value and change since range start, and a dashed baseline at the range start value; an allocation ring with a legend that dims other segments on hover; a rebalance card naming the exact dollar move with a 'Preview the trade' toggle that previews the after-trade mix in place; below, a holdings table with weight bars, quantities and gain/loss. Sage-grey ground, one deep-pine accent, green for gains and red only when something actually fell — the mood of a private bank statement, not a trading terminal.",
  "prompt_zh": "投资组合仪表盘：64px 衬线总资产大数字、可 scrub 的走势图+区间切换与虚线基线、配置环形图+图例悬停联动、写明具体金额的调仓卡（预览交易后配比）、持仓表带权重条，鼠尾草灰底+深松绿单强调色，私人银行对账单气质而非交易终端。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-25T09:30:00+08:00",
  "source": "Design Lounge《Portfolio dashboard》构建简报（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-25）；https://www.designlounge.live/p/fintech-portfolio-dashboard"
}
```

### 外卖订单追踪：地图骑手+42px 大字 ETA+四步进度 (`mobile-delivery-tracking`)

```json
{
  "id": "mobile-delivery-tracking",
  "title": "外卖订单追踪：地图骑手+42px 大字 ETA+四步进度",
  "category": "移动端App",
  "styles": [
    "外卖",
    "配送追踪",
    "地图"
  ],
  "scenario": "做外卖/快递订单追踪页，需要地图+骑手位置+ETA 倒计时时",
  "prompt": "Design a food delivery order-tracking screen: the top half is a flat stylized map with a thick frame, a courier dot riding a route from restaurant to home — driven part solid, remaining part dotted; the courier dot glides forward and the ETA counts down in real time. Below the map, the answer is the biggest thing on screen in 42px type: arrival clock time on one line, minutes remaining in the brand color on the next. A four-step progress bar — Confirmed, Preparing, On the way, Delivered — with the current step pulsing; a courier card with avatar initials, name, call and message buttons; a folding order summary and a 'Help with this order' link. Loud food-packaging look: cream paper, tomato red, near-black ink, heavy rounded type, 20px corners, no glass or blur.",
  "prompt_zh": "外卖订单追踪页：上半扁平地图+骑手圆点沿路线滑行（已走实线、未走虚线）、42px 大字 ETA（到达时刻+剩余分钟）、四步进度条当前步脉冲、骑手卡（电话/消息）+可折叠订单小票，奶油纸+番茄红+近黑墨水的包装风大字设计。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-25T09:30:00+08:00",
  "source": "Design Lounge《Phone order tracking》构建简报（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-25）；https://www.designlounge.live/p/phone-order-tracking"
}
```

### 心情日记 App：每日提示+情绪选择+情绪日历+趋势洞察 (`mobile-mood-journal`)

```json
{
  "id": "mobile-mood-journal",
  "title": "心情日记 App：每日提示+情绪选择+情绪日历+趋势洞察",
  "category": "移动端App",
  "styles": [
    "心情日记",
    "心理健康",
    "日记"
  ],
  "scenario": "做私密心情日记/情绪记录 App，需要每日打卡、情绪日历与趋势洞察时",
  "prompt": "Design a private mood journal and diary app for young adults seeking self-reflection: home opens with a time-aware daily prompt (morning intention, evening reflection, skippable), then a mood selector on a gentle emoji scale with soft animation, tags (grateful, anxious, happy…), an optional photo memory and a rich-text entry. A calendar month view shows mood-colored dots per day — tap to reread that entry — with a gentle ink-fill streak indicator. An insights tab shows mood trends over time as a line chart, most common tags and writing frequency; a gratitude section offers a daily 'three things' prompt and a gratitude jar that fills over time. Local-first with optional encrypted cloud backup, biometric lock, warm paper textures, soft ink colors, handwriting-inspired headers with a clean serif body and generous line height. No social features, no gamification of feelings, no ads, no unencrypted sync.",
  "prompt_zh": "心情日记 App：按时段的每日提示（晨间意图/晚间反思、可跳过）、表情情绪选择+标签+照片记忆与富文本、月历按情绪着色打点可回读、趋势折线图+常用标签+感恩罐，本地优先+加密备份+生物锁，暖纸质感+墨色+手写风标题，禁社交/禁情绪游戏化/禁广告。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-25T09:30:00+08:00",
  "source": "Mejba《Claude Prompt to Design a Mood & Diary Journal App Interface》（搜索结果原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-25）；https://www.mejba.me/prompts/mood-diary-journal-app-interface"
}
```

## 2026-11-26 · 公开渠道收集（跑步追踪/DAW/视频剪辑/设计系统文档站/保险理赔）

来源核对：跑步追踪见 Firevibe《Running Tracker》模板页（已打开原文核对：6 屏结构、深色+珊瑚橙 #FF5733、Barlow Condensed 数字、路线自绘动效）+ Vibecode Strava 克隆提示词；DAW 见 FlowState《Interface Overview》（已打开原文核对：走带条/音轨列表/时间线/底部四面板）+ audio-ui.dev DAW 组件库；视频剪辑见 JSBits《Design a Video Trimmer / Timeline Editor》（已打开原文核对：预览+胶片条时间线+入出点手柄+缩放+J/K/L/逐帧+多轨分割重排+导出）+ CapCut 官方 AI 视频工作流；设计系统文档站见 DesignZig《UI Design System & Component Library Generator》（已打开原文核对：原则/token/组件结构/文档要求/技术规范/治理五节模板，改写为文档站 UI 生成提示词）+ Lenka Studio Storybook 8 搭建；保险理赔见 webdevpuneet《Insurance Claim Status Card》（已打开原文核对：四步 stepper 三态区分、可折叠时间线、金额置顶）+ Topcoder Firefly 理赔门户与 State Farm 理赔追踪改版案例。以上 5 条均为库里没有的场景（跑步追踪/音乐制作/视频剪辑/设计系统文档站/保险理赔），只进待验证区；提示词按来源要点原创改写，标注「同类收集，非原作摘录」。设计系统文档站为新分类「设计系统」。已与正式库 69 条 + 待验证区去重无重复（跑步追踪与 mobile-health 的通用健康总览、DAW 与 music-player 的播放器、视频剪辑与播客后期的纯音频剪辑、设计系统文档站与 detail-* 单条规则、保险理赔与 banking-web/mobile-fintech 的银行/钱包首页场景均不同）。

#### 跑步运动追踪 App：实时配速+路线回放 (`mobile-running-tracker`)

```json
{
  "id": "mobile-running-tracker",
  "title": "跑步运动追踪 App：实时配速+路线回放",
  "category": "移动端App",
  "styles": [
    "运动追踪",
    "跑步",
    "深色",
    "数据仪表"
  ],
  "scenario": "做跑步 App，需要实时记录、配速分段与跑后路线回放时",
  "prompt": "Design a running tracker app (390x844): a Record screen with a live GPS route drawing itself on a dark map as you run, huge current pace in condensed bold numerals (Barlow Condensed style), elapsed time, distance and calories in a row below, and a big pause/stop control in the thumb zone; a run-summary screen with the full route map, per-kilometre splits table, elevation profile, pace-over-time chart and achievements badges; an Activities feed of friends' runs with route thumbnails, distance/pace/time stats and Kudos buttons that pop on tap. Deep near-black background #0D0D0F, coral-orange primary #FF5733 reserved for live data, actions and achievements only, carbon-fibre-like dark cards with razor-thin borders, Inter body text, energetic and precise like a Garmin watch face brought to life as a full app.",
  "prompt_zh": "跑步追踪 App：记录屏实时 GPS 路线自绘+超大当前配速数字、跑后总结含每公里分段表与海拔曲线、好友跑步动态带路线缩略图与 Kudos 点赞，深黑底+珊瑚橙只用于实时数据与成就。",
  "tools": [
    "v0",
    "Lovable",
    "即梦"
  ],
  "source": "Firevibe《Running Tracker》模板页（已打开原文核对：6 屏结构、深色+珊瑚橙 #FF5733、Barlow Condensed 数字、路线自绘动效；提示词按主题原创改写，同类收集，非原作摘录，2026-11-26）+ Vibecode Strava 克隆提示词（搜索结果核对：活动动态、路线回放、分段成绩）",
  "added_at": "2026-11-26T08:30:00+08:00"
}
```

#### 音乐制作 DAW：多轨时间线+混音台 (`daw-music-studio`)

```json
{
  "id": "daw-music-studio",
  "title": "音乐制作 DAW：多轨时间线+混音台",
  "category": "内容社交",
  "styles": [
    "音乐制作",
    "DAW",
    "深色",
    "专业工具"
  ],
  "scenario": "做音乐制作/编曲工具，需要多轨编排、鼓机与混音台同屏时",
  "prompt": "Design a desktop DAW (digital audio workstation) interface: top transport bar with play/stop/record, loop toggle, BPM readout (click to change 40-300), 4/4 time signature and metronome toggle; left track list with track name, M/S/R buttons (mute, solo, record-arm) and volume slider per track; centre timeline with a bars-and-beats ruler, white playhead, audio clips shown as waveforms on a beat grid, and a yellow-orange loop region; bottom tabbed panel with four tabs — Drums (16-pad drum machine with step sequencer and swing control), Mixer (channel strips with fader, pan, 3-band EQ, reverb/delay sends and a master channel with limiter), Samples (search samples by description, drag onto the timeline) and Vocal (autotune with key selection, compression, EQ and preset chains). Dark studio theme, one warm amber accent for the playhead and record-armed tracks, dense but organised like Ableton/FL Studio, every control reachable without nested menus.",
  "prompt_zh": "音乐制作 DAW：顶部走带条（播放/录音/循环/BPM/节拍器）、左侧音轨列表（静音/独奏/待命+音量）、中央波形时间线、底部鼓机/混音台/采样库/人声链四标签面板，深色录音棚风、琥珀色只标播放头与录音轨。",
  "tools": [
    "v0",
    "Cursor",
    "Lovable"
  ],
  "source": "FlowState DAW《Interface Overview》（已打开原文核对：走带条/音轨列表/时间线/底部四面板结构与各面板细节；提示词按主题原创改写，同类收集，非原作摘录，2026-11-26）+ audio-ui.dev DAW 组件库（搜索结果核对：编排时间线、钢琴卷帘、混音台通道条）",
  "added_at": "2026-11-26T08:30:00+08:00"
}
```

#### 视频剪辑时间线：预览+胶片条+多轨 (`video-editor-timeline`)

```json
{
  "id": "video-editor-timeline",
  "title": "视频剪辑时间线：预览+胶片条+多轨",
  "category": "内容社交",
  "styles": [
    "视频剪辑",
    "时间线",
    "创作工具",
    "深色"
  ],
  "scenario": "做视频剪辑工具，需要预览、裁剪与多轨时间线同屏时",
  "prompt": "Design a video editor interface (desktop, CapCut/Premiere style): top-left media bin with imported clips as thumbnails; centre video preview with transport controls (play/pause, J/K/L shuttle, frame step, timecode readout); bottom multi-track timeline with a time ruler, a thumbnail filmstrip under each video clip, a playhead synced to playback, draggable in/out trim handles on every clip, and separate tracks for video, audio, text/captions and transitions; a right panel switching between Effects, Transitions, Text, Stickers and Audio. Support split, reorder, delete and ripple edit on clips, zoom on the timeline (pixels-per-second), keyboard shortcuts shown in tooltips, and an Export button with resolution, frame rate and format options. Dark editing theme, one accent colour for the playhead and selected clip, precise and professional like a real NLE, no decorative gradients.",
  "prompt_zh": "视频剪辑器：左侧素材箱、中央预览+走带/逐帧/时间码、底部多轨时间线（标尺+缩略图胶片条+入出点手柄+视频/音频/字幕/转场分轨）、右侧特效面板，支持分割/重排/波纹编辑与缩放导出，深色专业剪辑风。",
  "tools": [
    "v0",
    "Cursor",
    "Lovable"
  ],
  "source": "JSBits《Design a Video Trimmer / Timeline Editor》（已打开原文核对：预览+胶片条时间线+入出点手柄+缩放+J/K/L/逐帧+多轨分割重排+导出；提示词按主题原创改写，同类收集，非原作摘录，2026-11-26）+ CapCut 官方 AI 视频工作流与 Dreamina 非线性编辑器（搜索结果核对：时间线卡片、字幕/音乐面板、片段自由裁剪重排）",
  "added_at": "2026-11-26T08:30:00+08:00"
}
```

#### 设计系统组件文档站：导航+展示+代码 (`design-system-docs-site`)

```json
{
  "id": "design-system-docs-site",
  "title": "设计系统组件文档站：导航+展示+代码",
  "category": "设计系统",
  "styles": [
    "设计系统",
    "组件文档",
    "文档站",
    "Storybook"
  ],
  "scenario": "给团队做设计系统文档站，需要组件展示、token 表与代码片段同站时",
  "prompt": "Design a design-system documentation website: left sidebar navigation grouped into Foundations (Color, Typography, Spacing, Icons, Elevation), Components (Button, Input, Card, Modal, Table, Toast) and Patterns (Forms, Navigation, Data display), with a search box at the top and the current page highlighted; main content shows one component per page — a live interactive preview with variant and state switchers (default, hover, active, disabled, error), a props table (name, type, default, description), a Do and Don't usage section with paired good/bad examples, and a copyable code snippet tab (React / Vue / plain HTML) with a copy button; a Tokens page displays the color palette with hex values and WCAG contrast ratios, the type scale and the spacing scale as swatch tables. Light theme, one brand accent, generous whitespace, monospace for code, clear hierarchy like Storybook docs or shadcn/ui — the site itself must demonstrate the system it documents.",
  "prompt_zh": "设计系统文档站：左侧分组导航（基础/组件/模式）+搜索、每组件一页（实时预览+五态切换、属性表、Do/Don't 正反示例、可复制代码片段）、token 页展示色板对比度与字阶间距，站本身就是系统的示范。",
  "tools": [
    "v0",
    "Cursor",
    "Lovable"
  ],
  "source": "DesignZig《UI Design System & Component Library Generator》（已打开原文核对：原则/token/组件结构/文档要求/技术规范/治理五节模板；提示词按模板要点原创改写为文档站 UI 生成提示词，同类收集，非原作摘录，2026-11-26）+ Lenka Studio《Storybook 8 组件库搭建》与 Strapi《Storybook + Next.js 设计系统》（搜索结果核对：autodocs、Controls 面板、MDX 文档页）",
  "added_at": "2026-11-26T08:30:00+08:00"
}
```

#### 保险理赔进度追踪：四步 stepper+时间线 (`fin-insurance-claim-tracker`)

```json
{
  "id": "fin-insurance-claim-tracker",
  "title": "保险理赔进度追踪：四步 stepper+时间线",
  "category": "金融",
  "styles": [
    "保险理赔",
    "进度追踪",
    "Stepper",
    "信任感"
  ],
  "scenario": "做保险理赔追踪页，用户只想一眼知道理赔到哪一步、还差什么时",
  "prompt": "Design an insurance claim tracking page: top card shows claim number, claim type (e.g. auto collision), filed date and the claim amount in large green numerals; below it a connected four-step stepper (Submitted → Under Review → Approved → Paid) where the line between two steps only fills in once the earlier step is complete, a completed step gets a filled dot, the current step gets a hollow dot with a soft glow halo — approved-but-not-yet-paid must look clearly different from paid; a 'Pending actions' inbox lists what the claimant still owes (upload photos, choose repair shop, confirm payout method), each marked Required or Recommended in words, not colour alone; a collapsible timeline below (closed by default, expands with a smooth max-height transition) holds the dated event history (assigned adjuster, inspection completed, approval); a message-the-adjuster button and an estimated completion date for the current step. Calm trustworthy palette (white, deep green or indigo accent), large readable text, no jargon, designed so the two questions 'how much' and 'how far along' are answered in the first half-second.",
  "prompt_zh": "保险理赔追踪页：顶部理赔单号/类型/金额、四步 stepper（连接线只随已完成步骤填色、进行中为空心光晕）、待办收件箱（必填/推荐用文字标明）、默认收起的日期事件时间线、联系理赔员入口与当前步骤预计完成日，金额与进度半秒内可读。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "source": "webdevpuneet《Insurance Claim Status Card》（已打开原文核对：四步 stepper 三态区分、可折叠时间线、金额置顶、页面自带重建提示词亦已核对；提示词按要点原创改写并扩展为完整追踪页，同类收集，非原作摘录，2026-11-26）+ Topcoder《Firefly Insurance Claims Status Portal》与 State Farm 理赔追踪改版案例（搜索结果核对：待办收件箱、理赔员沟通、任务可见性）",
  "added_at": "2026-11-26T08:30:00+08:00"
}
```

## 2026-11-26 · 公开渠道收集（空间 09:12 轮次：徒步路线/甘特图/退货售后/植物养护/帮助中心）

来源核对：徒步路线见 Brainy《Hiking Trail App Design: Trail Page Before and After》（三数分栏、海拔填色、路况一行、48px 开始按钮）与 open-design.ai《Offline Hiking Journal》提示词（搜索结果原文核对）；甘特图见 Routine《5 Prompts to Build a Gantt Chart With AI》（五条分工提示词）与 Techpresso《30 Claude Prompts That Build Gantt Charts》（搜索结果原文核对）；退货售后见 Snill《Build a Returns and RMA App》（六态生命周期、原因即数据）与 webdevpuneet《Return Label Generator》（两态卡片、原因下拉+按件勾选、确认页下一步，搜索结果原文核对）；植物养护见 blog.vibecoder.me《Build a Plant Watering Schedule App With AI》（四功能区四条提示词）与 MyPrompt 植物养护提醒 App UI 提示词、Crisp Leafwise 模板（搜索结果原文核对）；帮助中心见 VibeFather《Help Center Knowledge Base》模板（搜索优先首页+六分类+文章页目录/投票/相关文章）与 VibeWeek《In-Product Help Center & Knowledge Base》（搜索结果原文核对）。以上 5 条均为库里没有的页面/功能类型，只进待验证区；提示词按来源要点原创改写，标注「同类收集，非原作摘录」，不冒充原作逐字摘录。已与正式库 69 条 + 待验证区 92 条逐一去重：徒步路线与 mobile-running-tracker（跑步运动数据追踪）不同，是路线发现+海拔剖面+当日路况的出门前决策页；甘特图与 saas-kanban（看板列间拖拽）不同，是时间线+依赖+里程碑+关键路径视图；退货售后与 ecom-checkout-flow（下单到支付）不同，是售后退货流程；植物养护与 mobile-medication-reminder（用药提醒）同为提醒模式但场景不同（植物档案/浇水周期/养护日志/生长照片）；帮助中心与 saas-support-ticketing（工单人工处理）不同，是自助文档+AI 问答+转人工的帮助中心。

#### 户外徒步路线详情：三数分栏+海拔填色+路况一行 (`mobile-hiking-trail`)

```json
{
  "id": "mobile-hiking-trail",
  "title": "户外徒步路线详情：三数分栏+海拔填色+路况一行",
  "category": "移动端App",
  "styles": [
    "徒步",
    "户外",
    "路线详情",
    "地图"
  ],
  "scenario": "做徒步/户外 App 的路线详情页，用户出门前要快速判断这条线今天能不能走时",
  "prompt": "Design a hiking trail detail screen that answers 'is this the right trail today' in one glance: a full-width trail photo with the trail name in 24px bold and one quiet line under it (rating, difficulty, loop type, dogs allowed); three numbers a hiker compares between trails — distance, elevation gain and estimated time — each in its own column at 20px semibold with a small label beneath; an elevation profile drawn as a filled shape (light forest green fill, darker line on top, summit named with its height, start/end elevations at the bottom corners) instead of a thin grey line; conditions collapsed to a single 44px row with a chevron that warns about the one thing that matters today (e.g. mud after rain); one 48px Start Hike primary button plus two 48px circular secondary buttons (bookmark, share). Warm ivory background, forest green (#1F5E3B) accent, outdoor photography, generous spacing, large tap targets, offline-friendly — the facts a hiker came for must never be the smallest text on the page.",
  "prompt_zh": "徒步路线详情页：大图+24px 粗体路线名、三数分栏（里程/爬升/用时 20px 半粗体各占一列）、海拔画成填色形状并标出峰顶高度、路况缩成一行 44px 警示条、48px 开始徒步主按钮，米白+森林绿户外配色，关键数字绝不做成最小字。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "source": "Brainy《Hiking Trail App Design: Trail Page Before and After》（搜索结果原文核对：三数分栏、海拔填色形状、路况一行、48px 开始按钮；提示词按要点原创改写，同类收集，非原作摘录，2026-11-26）+ open-design.ai《Offline Hiking Journal》提示词（搜索结果核对：离线记录/同步队列、三屏结构）",
  "added_at": "2026-11-26T09:12:00+08:00"
}
```

#### 甘特图项目时间线：阶段分栏+依赖+关键路径 (`saas-gantt-chart`)

```json
{
  "id": "saas-gantt-chart",
  "title": "甘特图项目时间线：阶段分栏+依赖+关键路径",
  "category": "SaaS后台",
  "styles": [
    "甘特图",
    "项目管理",
    "时间线",
    "依赖"
  ],
  "scenario": "做项目管理工具的时间线/甘特图视图，需要阶段、依赖与关键路径同屏时",
  "prompt": "Design a Gantt chart project timeline view: left task list grouped into phases (Research, Design, Development, QA, Launch) with owner avatars and progress bars per task; right timeline grid with one row per task, one column per week, bars coloured per phase and a today line cutting across; dependencies drawn as arrows between bars, blocked tasks flagged in red with a short risk note; milestones as diamonds at phase ends; a critical-path toggle that highlights the chain of tasks that decides the launch date; a top bar to switch week/month zoom, filter by team (Engineering, Design, Marketing, QA) and show a mini progress summary (X of Y tasks done, N days to launch). When a date slips, dependent bars shift automatically and at-risk items surface in a side panel with suggested buffer time. Clean SaaS look, one accent colour per phase, readable at 100+ tasks without horizontal scrolling chaos — freeze the task list while the timeline scrolls.",
  "prompt_zh": "甘特图时间线：左侧阶段分组任务表（负责人+进度条）、右侧周列时间网格（阶段配色条+今日线）、依赖箭头与阻塞标红、里程碑菱形、关键路径开关、顶部周/月缩放与团队筛选，日期一拖依赖自动顺延、风险项进侧栏提示缓冲期。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "source": "Routine《5 Prompts to Build a Gantt Chart With AI》（搜索结果原文核对：阶段/依赖/风险点/多团队配色/里程碑 KPI 五条分工提示词；提示词按要点原创改写，同类收集，非原作摘录，2026-11-26）+ Techpresso《30 Claude Prompts That Build Gantt Charts》（搜索结果核对：多冲刺交付、依赖与评审里程碑、关键路径）",
  "added_at": "2026-11-26T09:12:00+08:00"
}
```

#### 电商退货/售后：原因即数据+六态生命周期 (`ecom-returns-refund`)

```json
{
  "id": "ecom-returns-refund",
  "title": "电商退货/售后：原因即数据+六态生命周期",
  "category": "电商零售",
  "styles": [
    "退货",
    "售后",
    "RMA",
    "流程"
  ],
  "scenario": "做电商售后退货页或商家退货管理后台，需要从申请到退款全程可查时",
  "prompt": "Design a product returns flow as two connected views. Customer side: start from the order, pick the items to return with a checkbox list (whole row clickable, size/quantity shown per item), choose a required reason from a short list (faulty, wrong item, changed mind, damaged, never arrived) and state the wanted outcome (refund, exchange or store credit) — the reason is stored as data, not a free-text note, so the shop can answer 'why are people returning this product'. Before submitting, show the policy branch: within the return window gets a label, final-sale items explain the exclusion and offer human help, damaged items ask for a photo and route to review. After submitting, a confirmation card shows the return number in large tabular numerals, a QR code or printable label, and numbered next steps (pack, drop off, refund timeline). Merchant side: a returns register with six states kept apart — requested, authorised, received, refunded, replaced, rejected — a waiting-to-be-received queue the warehouse cares about, and a return-rate-by-reason summary. Only a supervisor can reject. Clean, calm, honest copy: never promise a refund the policy does not allow.",
  "prompt_zh": "退货售后双面：用户侧从订单勾选退货商品+必选原因（原因存为数据）+选退款/换货/积分、按政策分支（在窗期内给面单、最终清仓品说明排除、破损要照片转人工），确认卡给退货号+二维码面单+分步指引；商家侧六态登记簿（申请/授权/已收/已退款/已换货/已拒绝）+待收队列+按原因退货率，拒绝仅主管可操作。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "source": "Snill《Build a Returns and RMA App — One Prompt, 48 Seconds》（搜索结果原文核对：六态生命周期、原因即数据、待收队列、仅主管可拒绝；提示词按要点原创改写，同类收集，非原作摘录，2026-11-26）+ webdevpuneet《Return Label Generator》（搜索结果核对：两态一卡片、原因下拉+按件勾选、确认页下一步）",
  "added_at": "2026-11-26T09:12:00+08:00"
}
```

#### 植物养护 App：今日待浇+一键记浇水+紧急度配色 (`mobile-plant-care`)

```json
{
  "id": "mobile-plant-care",
  "title": "植物养护 App：今日待浇+一键记浇水+紧急度配色",
  "category": "移动端App",
  "styles": [
    "植物养护",
    "提醒",
    "生活方式",
    "绿色"
  ],
  "scenario": "做植物养护/浇水提醒 App，家里植物总因浇水不规律养死时",
  "prompt": "Design a plant care app in a fresh green and cream palette: top greeting ('Good morning, Mia') with a small leaf avatar; a hero card with a monstera photo and a circular progress ring labelled 'Water in 2 days' plus a green 'Water Now' button; below, a 'Today's care' list of plant rows — each with a small round thumbnail, plant nickname, and the next action with its time window (e.g. 'Water today, Evening') — sorted by urgency with colour coding (red overdue, yellow due today, green upcoming); one tap on a plant logs the watering and moves its next date on, and a quick-action menu offers Water, Fertilize, Repot, Prune and Mist; a plant detail page shows its schedule, a care-history timeline and a strip of growth photos over time; a calendar tab shows the next fourteen days of care. A care-tip card reads 'Care tip: Rotate plants weekly for even growth'. Bottom tab bar: Home, Plants, Reminders, Profile. Clean spacing, rounded cards, real plant photos, legible short labels — and state plainly that schedules are user-supplied, not plant diagnoses.",
  "prompt_zh": "植物养护 App：问候+头像、主卡大图+浇水倒计时圆环+立即浇水按钮、今日养护列表按紧急度配色排序（逾期红/今日黄/将至绿）、一键记浇水自动顺延下次日期、详情页含养护时间线与生长照片、14 天养护日历，提醒是用户自定日程而非植物诊断。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "source": "blog.vibecoder.me《Build a Plant Watering Schedule App With AI》（搜索结果原文核对：植物档案/智能提醒/养护日志/推送四功能区与四条提示词；提示词按要点原创改写，同类收集，非原作摘录，2026-11-26）+ MyPrompt 植物养护提醒 App UI 提示词（搜索结果核对：问候区/倒计时圆环/今日养护列表/养护小贴士）+ Crisp Leafwise 模板（搜索结果核对：共享养护、今日列表一键记录、生长照片）",
  "added_at": "2026-11-26T09:12:00+08:00"
}
```

#### 帮助中心/知识库：搜索优先+六分类+文章页目录 (`saas-help-center-kb`)

```json
{
  "id": "saas-help-center-kb",
  "title": "帮助中心/知识库：搜索优先+六分类+文章页目录",
  "category": "SaaS后台",
  "styles": [
    "帮助中心",
    "知识库",
    "搜索优先",
    "自助服务"
  ],
  "scenario": "给 SaaS 产品做帮助中心，用户带着问题来、想 30 秒内找到答案时",
  "prompt": "Design a help center / knowledge base for a SaaS product, search-first: a home page with one large instant-search card at the top (focused within five seconds of arrival), a six-category grid below it with article counts per category, and a popular-articles strip; category pages list their articles with the search kept in context; article pages use a sticky table-of-contents rail, short skimmable sections with numbered steps in plain words, a 'Was this helpful?' vote with a thank-you state, related articles, and a contact-support panel that says honestly what happens next. Add an in-product '?' button in the app header that opens the same knowledge base as a slide-in sidebar (380-420px) with contextual article suggestions based on the page the user is on, plus AI-powered Q&A over the docs that cites its sources and falls back to ticket creation when uncertain. Calm utility look: warm white ground, ink text, one dependable blue accent, hairlines instead of heavy cards. Every article earns its place by being skimmable — a slightly annoyed customer mid-task should reach the step they need within thirty seconds, or a human in two clicks.",
  "prompt_zh": "帮助中心：搜索优先首页（大搜索框+六分类网格带文章数+热门文章）、分类页保留搜索上下文、文章页吸顶目录+可扫读分步正文+有用投票+相关文章+联系客服面板；产品内「?」按钮滑出同库侧栏并按当前页推荐文章，AI 问答引用来源、不确定时转工单，暖白底+墨字+一抹蓝的冷静工具风。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "source": "VibeFather《Help Center Knowledge Base》模板（搜索结果原文核对：搜索优先首页+六分类+文章页目录/投票/相关文章/联系面板；提示词按要点原创改写，同类收集，非原作摘录，2026-11-26）+ VibeWeek《In-Product Help Center & Knowledge Base》（搜索结果核对：产品内「?」侧栏、上下文推荐、AI 问答+来源引用、转人工兜底）",
  "added_at": "2026-11-26T09:12:00+08:00"
}
```

## 2026-11-27 · Motion Library 试收（8 候选，7 条进待验证区，1 条去重未收）

来源核对：Motion Library（https://kittenjam-motion-library.vercel.app/，2026-11-26 已批准为常驻收集来源）站上 8 个候选均已找到对应卡片并点「複製 AI 提示詞」取原文；提示词原文均为繁体中文，照录未改写。去重：按 id 与「场景+风格」与正式库 73 条 + 待验证区 93 条逐一比对——柔和上浮 Gentle Fade Up（No.125）与正式库 detail-staggered-entrance（错开入场：区块元素依次淡入上浮、间隔约 100ms、无弹跳）同场景同风格，仅参数级差异，按规则不重复收；其余 7 条无重复。7 条均为动效类、无来源视频，按旧法生成验证；本轮验证额度已用满（日历/结账/个人主页/404），7 条留待后续轮次验证。

#### Motion Library：打字机 Typewriter (`ml-typewriter`)

```json
{
  "id": "ml-typewriter",
  "title": "Motion Library：打字机 Typewriter",
  "category": "细节优化",
  "styles": [
    "打字机",
    "文字动效",
    "循环切换"
  ],
  "scenario": "标题/hero 文字想逐字打出再换句时",
  "prompt": "文字像打字機一樣一個字一個字出現在兩行，後面有閃爍的游標，打完停留後再快速逐字刪除，換成下一句繼續打。明體字、第二行較淡，打字約每字 0.14 秒。",
  "prompt_zh": "打字机文字动效：两行文字逐字打出、闪烁光标、停留后逐字删除换下一句，明体字、第二行较淡，每字约 0.14 秒。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T08:15:00+08:00",
  "source": "Motion Library No.064 打字機 Typewriter（https://kittenjam-motion-library.vercel.app/fx/64/，2026-11-27 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；参考来源 @ai_tjb「文字動態效果」；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：霓虹呼吸按钮 Neon Glow Button (`ml-neon-glow-button`)

```json
{
  "id": "ml-neon-glow-button",
  "title": "Motion Library：霓虹呼吸按钮 Neon Glow Button",
  "category": "细节优化",
  "styles": [
    "霓虹",
    "呼吸",
    "按钮",
    "悬停"
  ],
  "scenario": "按钮想做霓虹呼吸光晕、hover 强发光时",
  "prompt": "霓虹風格按鈕：外框細線與文字使用強調色，周圍有一圈柔和的外發光與內發光，光暈以約 2.4 秒的週期像呼吸般變亮又變暗；滑鼠滑過時整顆填滿、文字反白，並散發出多層大範圍的強烈光暈。（CSS：多層 box-shadow（含 inset）做發光，keyframes 改變光暈大小與透明度；hover 時停止呼吸動畫、改成更大的多層 box-shadow，transition 0.35 秒）",
  "prompt_zh": "霓虹呼吸按钮：外框细线+内外发光、光晕约 2.4 秒周期呼吸明暗，hover 填满反白并散发多层强光晕。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T08:15:00+08:00",
  "source": "Motion Library No.237 霓虹呼吸按鈕 Neon Glow Button（https://kittenjam-motion-library.vercel.app/fx/237/，2026-11-27 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：果冻弹跳按钮 Jelly Button (`ml-jelly-button`)

```json
{
  "id": "ml-jelly-button",
  "title": "Motion Library：果冻弹跳按钮 Jelly Button",
  "category": "细节优化",
  "styles": [
    "果冻",
    "弹跳",
    "按钮",
    "点击反馈"
  ],
  "scenario": "按钮 hover/点击想做 Q 弹果冻挤压回弹时",
  "prompt": "滑鼠滑過或點擊時，按鈕像果凍一樣先被橫向壓扁（寬 1.18、高 0.82），再縱向拉長（寬 0.85、高 1.15），之後幅度遞減地來回晃動幾次回到原狀，整段約 0.7 秒，Q 彈可愛。（CSS keyframes：依序 scale(1.18,.82) → (.85,1.15) → (1.08,.92) → (.97,1.03) → (1,1)；點擊觸發時先移除 class、強制 reflow 再加回，才能重播）",
  "prompt_zh": "果冻弹跳按钮：hover/点击先横向压扁再纵向拉长、幅度递减晃动回原状，约 0.7 秒，Q 弹。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T08:15:00+08:00",
  "source": "Motion Library No.232 果凍彈跳按鈕 Jelly Button（https://kittenjam-motion-library.vercel.app/fx/232/，2026-11-27 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：全息闪卡 Holographic Card (`ml-holographic-card`)

```json
{
  "id": "ml-holographic-card",
  "title": "Motion Library：全息闪卡 Holographic Card",
  "category": "细节优化",
  "styles": [
    "全息",
    "卡片",
    "3D倾斜",
    "悬停"
  ],
  "scenario": "收藏卡/作品卡想跟随鼠标 3D 倾斜、全息箔光流动时",
  "prompt": "一張收藏卡（上方圖片、下方標題與編號），跟著游標在 3D 空間中傾斜（最大約 13 度）；卡片表面有一層炫彩的全息箔光，箔光的位置跟著游標移動，傾斜越多箔光越明顯，另外還有一團柔和反光跟著游標位置；游標離開時卡片回正、箔光淡化。（CSS + JS：mousemove 計算游標在卡片上的相對位置 0~1，設定 rotateX/rotateY 與 CSS 變數 --px、--py；箔光層是 repeating-linear-gradient 的炫彩條紋、mix-blend-mode:color-dodge，background-position 用 --px/--py；反光層是 radial-gradient 疊 overlay；父層 perspective）",
  "prompt_zh": "全息闪卡：收藏卡跟随鼠标 3D 倾斜约 13 度，炫彩箔光与反光跟随角度流动，离开回正淡化。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T08:15:00+08:00",
  "source": "Motion Library No.287 全息閃卡 Holographic Card（https://kittenjam-motion-library.vercel.app/fx/287/，2026-11-27 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：卡片浮起 Hover Lift Card (`ml-hover-lift-card`)

```json
{
  "id": "ml-hover-lift-card",
  "title": "Motion Library：卡片浮起 Hover Lift Card",
  "category": "细节优化",
  "styles": [
    "卡片",
    "悬停",
    "上浮",
    "缩图放大"
  ],
  "scenario": "作品卡片列表 hover 想上浮加深阴影、缩图框内放大时",
  "prompt": "一排作品卡片（上方縮圖、下方標題與一條文字列）。滑鼠移到某張卡片上時，卡片往上浮起一點並出現更深更大的陰影，縮圖在原本的框內慢慢放大約 1.15 倍（框不變、圖被裁切）；滑鼠離開時平滑回到原位。約 0.45–0.6 秒，緩出。（CSS：卡片 transition transform 與 box-shadow，:hover 時 translateY(-8px)；縮圖外框 overflow:hidden，內層圖 transform:scale(1.14)）",
  "prompt_zh": "卡片浮起：hover 卡片上浮 translateY(-8px)、阴影加深，缩图框内放大 1.15 倍，0.45–0.6 秒缓出。（原文正文写 1.15 倍、CSS 写 scale(1.14)，照录未统一）",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T08:15:00+08:00",
  "source": "Motion Library No.112 卡片浮起 Hover Lift Card（https://kittenjam-motion-library.vercel.app/fx/112/，2026-11-27 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：液态玻璃翻牌 Liquid Glass Flip Card (`ml-liquid-glass-flip-card`)

```json
{
  "id": "ml-liquid-glass-flip-card",
  "title": "Motion Library：液态玻璃翻牌 Liquid Glass Flip Card",
  "category": "细节优化",
  "styles": [
    "液态玻璃",
    "翻牌",
    "3D",
    "卡片"
  ],
  "scenario": "玻璃卡片想按鼠标进入方向 3D 翻面、带棱镜光与光带扫过时",
  "prompt": "放在風景背景上的一張直式霧面玻璃卡片：透過卡片看到的背景被模糊、略微放大，像隔著一片厚玻璃；卡片邊緣有一圈細細的稜鏡彩光，表面有柔和高光並跟著游標位置移動。正面左上是小標籤、右上是翻面圖示、下方是標題；背面是說明文字與按鈕。游標從卡片哪一邊進入，卡片就往那個方向 3D 翻面（從左右進入沿垂直軸翻、從上下進入沿水平軸翻），翻轉時一條斜向光帶掃過、稜鏡光跟著旋轉、底下的影子在翻到側面時變窄；游標在卡片上移動時卡片微微傾斜，離開後以帶彈性的動作翻回正面。觸控裝置改成點一下翻面。沒有互動時每隔幾秒從隨機方向自動翻一次。（GSAP：rotateX／rotateY 用 elastic.out 補間，依進入點相對卡片中心的 dx、dy 決定方向；玻璃不用 backdrop-filter，而是在卡片內放一份對齊位置的背景副本加 blur、saturate、scale 當透鏡，避免 3D 中失效；稜鏡邊框用 conic-gradient 加 mask-composite 只留外框）",
  "prompt_zh": "液态玻璃翻牌：雾面玻璃卡按鼠标进入方向 3D 翻面，光带扫过、棱镜光旋转、带弹性翻回；与正式库 detail-liquid-glass（材质五要素配方）场景不同，本条是翻面交互。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T08:15:00+08:00",
  "source": "Motion Library No.332 液態玻璃翻牌 Liquid Glass Flip Card（https://kittenjam-motion-library.vercel.app/fx/332/，2026-11-27 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；参考来源 Framer Marketplace；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：逐字升起 Split Rise (`ml-split-rise`)

```json
{
  "id": "ml-split-rise",
  "title": "Motion Library：逐字升起 Split Rise",
  "category": "细节优化",
  "styles": [
    "逐字",
    "入场动画",
    "文字动效",
    "遮罩"
  ],
  "scenario": "标题文字想逐字从遮罩下方升起、停留再滑出时",
  "prompt": "文字拆成單字，每個字放在裁切遮罩內，依序從遮罩下方滑上來（每字間隔約 0.06 秒、強烈減速），停留後再往上滑出。（GSAP：SplitText type chars + mask，from yPercent:110，ease power4.out，stagger）",
  "prompt_zh": "逐字升起：文字拆成单字、每字在裁切遮罩内从下方滑上，间隔约 0.06 秒，停留后向上滑出。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T08:15:00+08:00",
  "source": "Motion Library No.076 逐字升起 Split Rise（https://kittenjam-motion-library.vercel.app/fx/76/，2026-11-27 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

## 2026-11-27 · 公开渠道收集（空间轮次：流媒体浏览/赛博朋克落地页/按钮层级/航班值机/团课预约）

来源核对：5 条来源页面均已打开全文核对，提示词按要点原创改写（同类收集，非原作摘录），不冒充原作逐字摘录；与正式库 73 条 + 待验证区 100 条逐一去重，无重复（航班值机与 mobile-flight-status 航班状态查询不同，是值机选座+登机牌流程；团课预约与 mobile-gym-workout-logger 健身记录打卡不同，是课表占位+名额/候补规则；流媒体浏览与 music-player 音乐播放器、video-editor-timeline 剪辑时间线场景不同）。只进待验证区，added_at 统一记本轮时间 2026-11-27T09:12:00+08:00。

#### 流媒体视频浏览页：深色影院风横排片库 (`content-streaming-browse`)

```json
{
  "id": "content-streaming-browse",
  "title": "流媒体视频浏览页：深色影院风横排片库",
  "category": "内容社交",
  "styles": [
    "流媒体",
    "深色",
    "横排片库"
  ],
  "scenario": "做视频点播/课程片库类产品，需要 Netflix 风格的浏览首页时",
  "prompt": "Design a streaming browse page in Netflix style: a near-black canvas (#0D0D0D) so poster art carries all the color; a top hero banner for one featured title with its name, short description, year and duration, and a large Play button; below it, horizontal scrollable rows grouped by category (Trending, Originals, Top Rated), each row with the category name above and title cards showing thumbnail, name and a Play icon on hover — rows bleed off the right edge so a partial card hints at more, and on mobile cards are 140px wide with snap scrolling. Add a 'Continue Watching' row with a progress bar on each card, a title detail view with the poster as a large hero background under a gradient overlay plus metadata and a Related row, and a full-screen search overlay filtering by title with an empty state when nothing matches. Keep the chrome minimal: a slim top nav with logo, search icon and avatar; Inter for headings and body; one accent color for the Play button and active states.",
  "prompt_zh": "流媒体浏览页：近黑底色+海报即导航，顶部精选横幅配大播放键，下方按分类横排滚动片库（右侧溢出暗示更多），续看行带进度条、详情页渐变海报+相关推荐、全屏搜索带空态。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T09:12:00+08:00",
  "source": "Greta《Build a Netflix Clone with AI in 30 Minutes》（浏览页/详情页/搜索提示词原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-27）"
}
```

#### 赛博朋克风落地页：霓虹终端 HUD (`landing-cyberpunk`)

```json
{
  "id": "landing-cyberpunk",
  "title": "赛博朋克风落地页：霓虹终端 HUD",
  "category": "落地页官网",
  "styles": [
    "赛博朋克",
    "霓虹",
    "深色"
  ],
  "scenario": "给极客/游戏/加密类产品做一张霓虹科幻风落地页时",
  "prompt": "Design a cyberpunk landing page: a pure dark-first canvas (#0D0D0D) with neon accents covering only 10-15% of the surface — matrix green #00FF00, magenta #FF00FF and cyan #00FFFF, each color assigned a fixed meaning (one for CTAs, one for data, one for alerts) and never swapped. Monospace type throughout for the terminal feel (bold tight-tracked headings, 16px/1.6 body), with HUD overlays, stat readouts and coordinate displays treated as decoration that is also information; one controlled glitch effect per view at most (chromatic aberration or a 0.3s skew glitch), a subtle scanline overlay at 0.1 opacity, angular clipped shapes and zero or near-zero border radius. Page structure: navbar with logo, links and CTA; asymmetric hero with a huge headline, subtitle, two buttons and an abstract CSS visual; features as an asymmetric grid (never three equal columns); testimonials, three-tier pricing with the middle tier highlighted, a final CTA and a full footer. Dark mode only — no light variant; neon glow via text-shadow, no emojis, Lucide-style line icons only.",
  "prompt_zh": "赛博朋克落地页：#0D0D0D 纯黑底、霓虹三色各有固定语义且只占 10-15% 面积、等宽终端字体+HUD 数据叠层、每屏至多一个克制故障特效、扫描线 0.1 透明度、非对称布局，专供极客/游戏/加密类产品。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T09:12:00+08:00",
  "source": "designmd.app《Cyberpunk UI》DESIGN.md（配色/字体/动效/落地页结构原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-27）"
}
```

#### 按钮层级五级制：每屏只一个主按钮 (`detail-button-hierarchy`)

```json
{
  "id": "detail-button-hierarchy",
  "title": "按钮层级五级制：每屏只一个主按钮",
  "category": "细节优化",
  "styles": [
    "按钮",
    "层级",
    "组件规范"
  ],
  "scenario": "界面上按钮全是同款填充色、用户不知道先点哪个时",
  "prompt": "Apply a five-level button hierarchy with exactly one primary action per view (One Primary Action): Primary — the single filled, full-saturation button carrying the action that moves the user's main job forward ('Create project', 'Save changes'), one per view, never two; Secondary — outlined or lightly tinted fill with colored text for supporting actions ('Cancel' next to 'Save'); Tertiary — no fill, no border, colored text only, for low-stakes actions ('Skip for now', 'Learn more'); Ghost — the quietest interactive element, transparent background with neutral text and a faint hover state, for toolbar icons, dismiss controls and table row actions; Destructive — orthogonal to the ladder, a meaning not a loudness: red signals consequence and can sit at any level (filled red in a confirm dialog, quiet red text in a list). Ship all six states for every level: default, hover (slightly darker/lighter), focus-visible (a visible 2px focus ring with 2px offset — never remove the outline without replacing it), active (a touch darker, translateY 1px), disabled (muted, no pointer, no hover) and loading (spinner plus aria-busy, locked against double-submit). Sizes on the 8pt grid — sm 6px 12px/13px, md 10px 16px/14px, lg 14px 24px/16px; every hit target at least 44x44px even if the visual is smaller; 16px gaps between buttons (8px when stacked). Label the outcome, not the mechanism: 'Send invite', not 'Submit'.",
  "prompt_zh": "按钮五级制：每屏只一个填充主按钮（推进主任务的动作），其余降级为描边次要/纯文字三级/最安静幽灵按钮，危险色是语义而非音量；六态齐全（默认/悬停/可见焦点环/按下/禁用/加载防重复提交），三档尺寸走 8pt 网格、点击热区不小于 44px，文案写结果不写机制。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T09:12:00+08:00",
  "source": "hesham.us《Buttons: The Atom of the Interface》（五级层级/每屏一主按钮/六态/尺寸与热区原文核对）+ PatternFly Button 设计指南（主/次/三级/链接按钮层级与间距原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-27）"
}
```

#### 航班值机：选座+登机牌两屏 (`mobile-flight-checkin`)

```json
{
  "id": "mobile-flight-checkin",
  "title": "航班值机：选座+登机牌两屏",
  "category": "移动端App",
  "styles": [
    "值机",
    "登机牌",
    "选座"
  ],
  "scenario": "做航司 App 的在线值机流程，需要从确认乘客到登机牌的完整两屏时",
  "prompt": "Design a mobile airline check-in flow as two screens. Screen 1 — Check-in: a check-in status badge and a flight summary (route, date, flight number, departure/arrival local times on a 24-hour clock with terminals); passenger rows each showing name and a 'passport checked' line; a seat map grid for the cabin (3-3 on narrow-body) with five seat states — available, selected, reserved, extra legroom, exit-row disabled — plus a legend, per-passenger seat assignment, and a 120-second hold countdown once a seat is picked; optional extras (checked bags, priority boarding) as add-on rows with prices, then one primary 'Confirm check-in' button. Screen 2 — Boarding pass: a ticket-style card with the airline wordmark and booking reference (with copy button), big airport codes with local times and a dashed route line with a plane icon and flight duration, gate, date, seat and class, and a scannable code area at the bottom; wallet ('Add to Wallet') and share buttons below. Keep the pass legible offline at the gate: high contrast, no reliance on color alone to convey seat state, and all times shown in each airport's own local time.",
  "prompt_zh": "航班值机两屏：值机屏（状态徽章+航程摘要+乘客护照已核行+五态座位图+120 秒锁座倒计时+行李附加项）→登机牌卡（航司+预订号可复制、大字机场代码与本地时间、登机口座位舱位、可扫码区、加钱包/分享），离线可读、不只靠颜色区分座位态。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T09:12:00+08:00",
  "source": "ProFigma《Boarding Pass and Check-in Screens UI》（值机屏/登机牌两屏构成原文核对）+ UIReady《Design an Airline Seat-Selection UI》（座位五态/临时锁座/无障碍原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-27）"
}
```

#### 健身团课预约：课表+名额+候补 (`mobile-fitness-class-booking`)

```json
{
  "id": "mobile-fitness-class-booking",
  "title": "健身团课预约：课表+名额+候补",
  "category": "移动端App",
  "styles": [
    "团课预约",
    "课表",
    "健身"
  ],
  "scenario": "给健身房/瑜伽/普拉提工作室做团课预约 App，课有名额上限、要管候补和课包时",
  "prompt": "Build a fitness class booking app around a weekly timetable with a live counter on every class: each class row shows class type, coach (with photo), time, duration, room, and spots left out of capacity — capacity set by what actually limits it (15 mats, 24 bikes in four rows, 10 reformers), and for spin/Pilates let members pick a specific bike or mat spot from a room map. Filters by class type, coach and time of day; a class detail page with places left, a Book button, and a waitlist when full — when someone cancels, the first person on the waitlist is promoted automatically with a push notification, up to a cutoff (e.g. 1 hour before class), after which the spot stays open for walk-ins. Payment by drop-in, class packs (e.g. 10-class pack, 3-month expiry) or unlimited monthly membership, with a visible credit balance that drops per booking; cancellation before the cutoff returns the credit, later cancels and no-shows lose it. A 'My bookings' screen lists upcoming and past bookings with cancel and add-to-calendar actions, and coaches get a per-class check-in list with client notes (e.g. injuries). Keep booking to a few taps and never let a full class accept a booking silently.",
  "prompt_zh": "团课预约：周课表每节课带实时剩余名额（名额按垫子/单车/器械数定，动感单车可选具体车位），满员进候补（有人取消按序自动递补+推送，截止前 1 小时停止递补）、课包余额随订课扣减（截止前取消返还、逾期与爽约扣课时）、教练端点名表带学员备注。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-27T09:12:00+08:00",
  "source": "Gappsy《Fitness Class Booking Prompts: 12 Studio Ideas》（课表名额/按器械定容量/候补递补/取消扣课时规则原文核对）+ GrowApps《How to make a gym class booking app with AI》（课表/课包余额/教练点名表原文核对；提示词按要点原创改写，同类收集，非原作摘录，2026-11-27）"
}
```

## 2026-11-28 · Motion Library 收集（5 候选，4 条进待验证区，1 条去重未收）

来源核对：Motion Library（https://kittenjam-motion-library.vercel.app/，常驻收集来源）站上 5 个候选均已打开详情页点「複製 AI 提示詞」取原文；提示词原文均为繁体中文，照录未改写。去重：按 id 与「场景+风格」与正式库 77 条 + 待验证区 101 条逐一比对——骨架载入 Skeleton Shimmer（No.114）与待验证区 detail-skeleton-loading（骨架屏加载占位：与真实内容同尺寸同间距的灰块占位、1.4 秒柔和微光按列错峰扫过、数据一到逐块替换）同场景同风格，仅载体（整页 vs 单卡片）与入场细节级差异，按规则不重复收；其余 4 条无重复。4 条均为动效类、无来源视频，按旧法生成验证；本轮验证额度已用满（通知中心/搜索筛选/学习仪表盘/博客阅读），4 条留待后续轮次验证。通知堆叠与正式库 saas-notification-center（通知双面系统整页）场景不同：前者是 Toast 进退场动效，后者是通知系统页面，保留。

#### Motion Library：选单滑块跟随 Sliding Nav Highlight (`ml-sliding-nav-highlight`)

```json
{
  "id": "ml-sliding-nav-highlight",
  "title": "Motion Library：选单滑块跟随 Sliding Nav Highlight",
  "category": "细节优化",
  "styles": [
    "导航滑块",
    "悬停跟随",
    "胶囊导航"
  ],
  "scenario": "导航栏想让选中态滑块跟随鼠标平滑滑动时",
  "prompt": "膠囊形導覽列，滑鼠移到某個項目時，一顆膠囊背景滑塊從原本位置平滑滑過去並改變寬度貼合該項目，文字同時切換成與滑塊反差的顏色；滑鼠離開整個選單時滑塊回到目前所在的頁面項目。約 0.4 秒，帶一點點過衝。（做法：pointerenter 時讀取項目的 offsetLeft 與 offsetWidth，設定滑塊的 translateX 與 width，transition cubic-bezier(.2,.9,.3,1.1)）",
  "prompt_zh": "胶囊导航滑块跟随：鼠标移到某项，胶囊背景滑块平滑滑过去并贴合该项宽度、文字切换反差色，离开菜单滑回当前页项目，约 0.4 秒带一点过冲。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-28T08:05:00+08:00",
  "source": "Motion Library No.167 選單滑塊跟隨 Sliding Nav Highlight（https://kittenjam-motion-library.vercel.app/fx/167/，2026-11-28 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：步骤进度条 Step Progress (`ml-step-progress`)

```json
{
  "id": "ml-step-progress",
  "title": "Motion Library：步骤进度条 Step Progress",
  "category": "细节优化",
  "styles": [
    "步骤指示",
    "多步骤表单",
    "进度线"
  ],
  "scenario": "多步骤表单（注册/结账）上方需要步骤指示时",
  "prompt": "多步驟表單（例如註冊或結帳）上方的步驟指示：一排圓形步驟編號以一條線連接，已完成的步驟圓點填滿並以回彈出現勾勾，目前這一步外圈亮起並略為放大，未到的步驟維持淡色；連接線的填滿長度跟著步驟平滑延伸；下方有「上一步／下一步」按鈕。（CSS：連接線內層 transform:scaleX(目前索引 / (總數 − 1))，transition 0.5 秒；步驟以 .done / .on class 切換樣式，勾勾用 scale 0 → 1 的 keyframes）",
  "prompt_zh": "步骤进度条：圆形步骤编号以连线连接，已完成填满并回弹出现勾勾、当前步外圈亮起略放大、未到步骤淡色，连接线填满长度随步骤平滑延伸，配上一步/下一步按钮。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-28T08:05:00+08:00",
  "source": "Motion Library No.309 步驟進度條 Step Progress（https://kittenjam-motion-library.vercel.app/fx/309/，2026-11-28 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：通知堆叠 Toast Stack (`ml-toast-stack`)

```json
{
  "id": "ml-toast-stack",
  "title": "Motion Library：通知堆叠 Toast Stack",
  "category": "细节优化",
  "styles": [
    "通知堆叠",
    "Toast",
    "进退场"
  ],
  "scenario": "操作完成需要右下角弹出可堆叠的通知时",
  "prompt": "操作完成時，畫面右下角彈出一則通知（左邊打勾圓形圖示、中間訊息、右邊「剛剛」時間），從下方帶一點縮放彈性地進場；新通知會疊在下面，舊的往上推；最多同時顯示 3 則，每則約 3.4 秒後往右滑出淡掉，其餘通知平滑補位。（CSS + JS：通知外層用 display:grid + grid-template-rows 1fr→0fr 做高度收合，讓補位平滑；進場用 keyframes translateY + scale；離場加 .out class 後再移除元素）",
  "prompt_zh": "通知堆叠：右下角弹出通知（勾选图标+讯息+时间），带缩放弹性进场、新通知叠在下面旧的往上推，最多 3 则、约 3.4 秒后右滑淡出、其余平滑补位。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-28T08:05:00+08:00",
  "source": "Motion Library No.118 通知堆疊 Toast Stack（https://kittenjam-motion-library.vercel.app/fx/118/，2026-11-28 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```

#### Motion Library：滑动确认 Slide to Confirm (`ml-slide-to-confirm`)

```json
{
  "id": "ml-slide-to-confirm",
  "title": "Motion Library：滑动确认 Slide to Confirm",
  "category": "细节优化",
  "styles": [
    "滑动确认",
    "拖曳手势",
    "确认操作"
  ],
  "scenario": "支付/删除等高风险操作需要滑动确认防误触时",
  "prompt": "膠囊形滑軌，左側是一顆圓形把手（內有向右箭頭），中間的提示文字有一道光從左往右掃過；使用者拖曳把手時，把手經過的軌道被填滿、提示文字逐漸淡出；拖到接近最右側放開才算確認，軌道整個填滿、文字變成「完成 ✓」；未拖到底放開時把手帶彈性彈回起點。（GSAP Draggable type:\"x\"、bounds 限制在軌道內，onDrag 更新填滿寬度，onRelease 判斷是否超過 85%；流光用 background-clip:text 加移動的漸層）",
  "prompt_zh": "滑动确认：胶囊滑轨+圆形把手，拖曳时轨道填满、提示文字淡出，拖到 85% 以上放开才确认、文字变“完成 ✓”，未拖到底弹性弹回起点。",
  "tools": [
    "v0",
    "Lovable",
    "Cursor"
  ],
  "added_at": "2026-11-28T08:05:00+08:00",
  "source": "Motion Library No.234 滑動確認 Slide to Confirm（https://kittenjam-motion-library.vercel.app/fx/234/，2026-11-28 打开详情页点「複製 AI 提示詞」取原文；原文为繁体中文，照录；站上注明复制时会自动附加「依照網站既有主題色搭配」说明，该附加句未在页面显示；该站无源码与授权说明，只当收集来源与参考）"
}
```
