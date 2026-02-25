# UI_GUIDELINES: 简易任务管理系统

## 1. 风格定位
- **Bento Grid (便当盒风格)**：卡片化布局，整洁有序。
- **微交互**：按钮点击有缩放感，列表切换有淡入淡出动画。

## 2. 色彩规范 (Color Palette)
- **Primary**: `#3B82F6` (科技蓝)
- **Background**: `#F9FAFB` (浅灰白)
- **Text**: `#111827` (深色文字)
- **Success**: `#10B981` (翠绿)
- **Error**: `#EF4444` (警示红)
- **Warning**: `#F59E0B` (亮橙)

## 3. 间距规范 (Spacing)
- 基准单位: `4px` (Tailwind 默认单位)
- 内边距 (Padding): `16px (p-4)`, `24px (p-6)`
- 圆角 (Radius): `12px (rounded-xl)`, `16px (rounded-2xl)`

## 4. 字体规范 (Typography)
- **标题**: `font-bold`, `tracking-tight`
- **正文**: `font-normal`, `text-slate-600`
- **默认字体**: `system-ui, -apple-system, sans-serif`

## 5. 响应式断点 (Breakpoints)
- **Mobile First 策略**: 默认样式针对移动端。
- **Tablet (md)**: `768px` - 启用侧边栏，网格转为 2 列。
- **Desktop (lg)**: `1024px` - 网格转为 3 列，显示完整导航。
- **Wide (xl)**: `1280px` - 最大内容宽度限制。

## 6. 组件交互状态 (Interaction States)
- **Button**:
  - `Hover`: 背景色亮度降低 10% (`hover:bg-blue-600`)。
  - `Active`: 缩放 95% (`active:scale-95`)。
  - `Disabled`:不仅要变灰 (`opacity-50`)，还必须禁止 `cursor-not-allowed`。
- **Input**:
  - `Focus`: 蓝色外发光环 (`ring-2 ring-blue-500`)。
  - `Error`: 红色边框 (`border-red-500`)。

## 7. 资源管理 (Assets)
- **Icons**: 统一使用 `lucide-react`，大小默认为 `w-5 h-5`。
- **Images**: 必须使用 `next/image` 组件，禁止使用原始 `<img>` 标签。
