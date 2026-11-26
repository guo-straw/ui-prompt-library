# SaaS后台

## Linear 风 SaaS 数据后台 (`saas-dashboard-linear`)

- 风格：极简 / 深色 / 专业
- 场景：项目管理/协作类 SaaS 首页仪表盘
- 适用工具：v0、Lovable、Cursor

**EN prompt（复制用）**

```
Design a clean SaaS analytics dashboard in the style of Linear: dark sidebar navigation, light content area, compact data tables, KPI cards with sparklines, a line chart and a bar chart, status badges, subtle borders instead of heavy shadows, 8px spacing system, Inter font, primary color indigo #5E6AD2, rounded-lg corners, professional and information-dense but uncluttered.
```

**中文说明**：Linear 风极简 SaaS 仪表盘：深色侧边栏、紧凑表格、KPI 卡片+迷你趋势图、状态徽章、细边框少阴影、靛蓝主色、信息密集但不乱。

## 浅色企业管理系统 (`saas-admin-light`)

- 风格：浅色 / 企业级 / 表格密集
- 场景：订单/用户/权限等后台管理 CRUD
- 适用工具：v0、Cursor、Qoder

**EN prompt（复制用）**

```
Build an enterprise admin panel UI: top header with search and user avatar, left collapsible menu, breadcrumb, filter bar with date range and dropdowns, a paginated data table with row selection, status pills and action buttons, a slide-over detail drawer and a modal form. White and light gray palette, blue primary #1677FF, clear hierarchy, designed for daily heavy use, no decorative gradients.
```

**中文说明**：企业级浅色后台：顶栏+可折叠菜单、筛选条、分页表格、状态标签、详情抽屉和弹窗表单，蓝色主色，耐看实用不要花哨渐变。

## 看板协作工具 (`saas-kanban`)

- 风格：卡片 / 协作 / 彩色标签
- 场景：任务看板/项目进度管理
- 适用工具：v0、Lovable

**EN prompt（复制用）**

```
Create a Kanban project board UI like Trello/Linear: horizontal columns (Backlog, In Progress, Review, Done) with drag-ready cards, each card shows title, colored labels, assignee avatars, due date and comment count; top bar with board switcher, filter and members; soft gray background #F4F5F7, white cards with subtle shadow, friendly but professional.
```

**中文说明**：看板协作 UI：横向列+可拖拽卡片，卡片带彩色标签、成员头像、截止日期，浅灰底白卡片。

## 设置页主从布局 (`saas-settings-master-detail`)

![生成验证效果图](../previews/saas-settings-master-detail.png)

生成验证：✅ 2026-11-17 通过 — 生成图为设置页：左侧六项导航 Notifications 高亮，右侧分组卡片行式设置（左标题说明、右开关/下拉），底部 Unsaved changes 吸底条与红色 Danger zone 卡片均出现，通过

- 风格：主从布局 / 表单 / 设置
- 场景：产品设置/账户/团队管理页
- 适用工具：v0、Cursor、Lovable

**EN prompt（复制用）**

```
Design a settings page in a master-detail layout: left vertical nav (Profile, Account, Notifications, Billing, Security, Team) with the active item highlighted; right panel shows the active section as grouped cards, each setting as one row — title and helper text on the left, the control (toggle, select or button) on the right, comfortable 56px row height. Save per section and show a sticky 'Unsaved changes' bar at the bottom only when edits are pending. Put destructive actions in a separate red-bordered 'Danger zone' card at the very bottom. Calm neutral palette, one accent, no endless ungrouped scroll.
```

**中文说明**：设置页主从布局：左侧分组导航、右侧按卡分组的设置行（标题+说明+右侧控件）、有改动才吸底保存条、危险操作单独红框放最底。

## SpicyTater：后台菜单交互 8 类选型 (`spt-admin-menu`)

![生成验证效果图](../previews/spt-admin-menu.png)

生成验证：✅ 2026-11-19 通过 — 生成图为 Orbit 后台：滑动高亮块选中 Dashboard、Projects 就地展开子菜单、顶部页签带高亮、⌘K 命令面板搜索条、Inbox 12 徽标+状态点、底部悬浮停靠栏齐全，通过

- 风格：后台菜单、交互选型、章节摘录
- 场景：做后台/侧栏导航菜单，不知道用哪种展开方式时
- 适用工具：v0、Lovable、Cursor

**EN prompt（复制用）**

```
Choose admin menu patterns by structure: sliding highlight block for sidebar nav and top tabs; expand-in-place submenus for hierarchical project/file trees; top drop-down panel when there are few sections but multiple entries (mouse and keyboard); floating bottom dock for frequent entries (magnify on hover, neighbours make room); command palette when entries are many (search + keyboard selection); status dots and count badges for new messages and pending items, animating the number when it changes. Pick the combination by section count, hierarchy depth and usage frequency; entries must stay obvious and reachable.
```

**中文说明**：SpicyTater 第22集（2062赞）：滑动高亮块/就地展开/顶部下落面板/底部悬浮停靠栏/命令面板/状态点徽标等 8 类后台菜单，按栏目数量、层级、频率选组合。

## 费纸张：设置页三步排版（原作版） (`saas-settings-three-steps`)

![生成验证效果图](../previews/saas-settings-three-steps.png)

生成验证：✅ 2026-11-22 通过 — 生成图为 Acme 设置页：一项一行（左名右控件）、无最外层卡片框、Profile/Notifications/Billing 分组加标题且组间留白大于组内、行间细线分隔，三步全部呈现，通过（Timezone 一处拼写为 Tizezone，小瑕疵）

- 风格：设置页、排版、原作摘录
- 场景：AI 做的设置页杂乱、框套框时
- 适用工具：v0、Lovable、Cursor

**EN prompt（复制用）**

```
Lay out this settings page in three steps: 1) one setting per row — name on the left, control on the right; 2) remove the outermost frame — the page itself needs no extra card wrapper; 3) group settings under group titles with generous spacing between groups, tight spacing within groups and only hairline dividers between rows. Note: for registration/checkout forms instead put labels above full-width inputs, in fill order, leaving room for error messages and longer content.
```

**中文说明**：费纸张第5集原作三步：一项一行（左名右控件）、去掉最外层框、分组加标题（组间多留白、组内少留白、行间细线）；并对比表单场景：名称在上、全宽输入。与设置页主从布局同属设置页风格组。

## 登录页：社交登录优先+单主按钮 (`auth-login-page`)

![生成验证效果图](../previews/auth-login-page.png)

生成验证：✅ 2026-11-26 通过 — 生成图为 SaaS 登录页：Google/Apple/GitHub 三按钮在前、Passkey/Magic Link、or with email 分隔线、邮箱+单个密码框带显示切换、密码旁 Forgot password?、具体报错文案'That password is not right. Reset it'、蓝色 Log in 主按钮带加载态'Logging in...'、按钮下隐私说明与 New here? Create an account 链接、左上 Back to site，中性底+单强调色、无紫色渐变，通过

- 风格：登录 / 表单 / 极简
- 场景：做登录页、默认模板总把注册和登录混在一起时
- 适用工具：v0、Lovable、Cursor

**EN prompt（复制用）**

```
Design a login page for a SaaS product: sign-in providers first — Google, Apple and GitHub buttons plus a passkey/magic-link option above an 'or with email' divider, so most returning users never type a password. The form: email and one password field with a show-password toggle; no confirm-password field. One primary action: a single solid Log in button; demote sign up to a quiet 'New here? Create an account' link. A 'Forgot password?' link right beside the password field. Specific error copy ('That password is not right. Reset it') and a loading state on the button. Style: neutral base, one accent color on the primary button only, named headline/body typefaces, no purple gradient. A short privacy note under the button and a clear path back to the marketing site.
```

**中文说明**：登录页：社交/密钥登录放最前、邮箱+单个密码框带显示切换、一个 Log in 主按钮、注册降级为链接、密码旁放找回链接、写清具体报错与加载态，中性底+单强调色。
