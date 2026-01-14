# Theme System - Developer Quick Reference

This guide shows how to use the centralized theme system with Tailwind CSS v4.

## ✅ DO - Use Theme Tokens

### Backgrounds
```tsx
// ✅ Good - uses theme token
<div className="bg-card">Content</div>
<div className="bg-primary">Button</div>
<div className="bg-[var(--background)]">Custom</div>

// ❌ Bad - hardcoded color
<div className="bg-white dark:bg-gray-800">Content</div>
```

### Text Colors
```tsx
// ✅ Good
<p className="text-foreground">Main text</p>
<p className="text-foreground-secondary">Secondary text</p>
<p className="text-foreground-muted">Muted text</p>

// ❌ Bad
<p className="text-gray-900 dark:text-white">Text</p>
```

### Buttons
```tsx
// ✅ Primary Button
<button className="bg-primary hover:bg-primary-hover text-primary-foreground">
  Click me
</button>

// ✅ Secondary Button
<button className="bg-secondary hover:bg-secondary-hover text-secondary-foreground">
  Cancel
</button>

// ✅ Success Button
<button className="bg-success hover:bg-success-hover text-success-foreground">
  Save
</button>

// ✅ Danger Button
<button className="bg-error hover:bg-error-hover text-error-foreground">
  Delete
</button>
```

### Borders
```tsx
// ✅ Good
<div className="border border-[var(--border)] hover:border-[var(--border-hover)]">
  Card
</div>

// Focus ring
<input className="focus:ring-2 focus:ring-[var(--border-focus)]" />
```

### Cards
```tsx
// ✅ Good
<div className="bg-card text-card-foreground border border-[var(--border)] hover:bg-card-hover">
  Card content
</div>
```

### Alert Messages
```tsx
// ✅ Success
<div className="bg-success-light border-l-4 border-success text-foreground">
  <svg className="text-success">✓</svg>
  Success message
</div>

// ✅ Error
<div className="bg-error-light border-l-4 border-error text-foreground">
  <svg className="text-error">✗</svg>
  Error message
</div>

// ✅ Warning
<div className="bg-warning-light border-l-4 border-warning text-foreground">
  <svg className="text-warning">⚠</svg>
  Warning message
</div>
```

## 📋 Available Theme Classes

### Colors
- `bg-primary`, `bg-primary-hover`, `bg-primary-light`
- `bg-secondary`, `bg-secondary-hover`, `bg-secondary-light`
- `bg-accent`, `bg-accent-hover`, `bg-accent-light`
- `bg-success`, `bg-success-hover`, `bg-success-light`
- `bg-error`, `bg-error-hover`, `bg-error-light`
- `bg-warning`, `bg-warning-hover`, `bg-warning-light`
- `bg-card`, `bg-card-hover`
- `bg-muted`
- `bg-disabled`

### Text Colors
- `text-foreground` (main text)
- `text-foreground-secondary` (secondary text)
- `text-foreground-muted` (subtle text)
- `text-primary-foreground` (text on primary backgrounds)
- `text-card-foreground` (text on cards)
- `text-success`, `text-error`, `text-warning`

### Navigation & Footer
- `bg-nav-background`, `text-nav-foreground`
- `text-nav-link`, `text-nav-link-hover`, `text-nav-link-active`
- `bg-footer-background`, `text-footer-foreground`
- `text-footer-link`, `text-footer-link-hover`

## 🎨 Using CSS Variables Directly

For one-off cases or when you need more control:

```tsx
<div style={{ backgroundColor: 'var(--primary)' }}>
  Custom styled element
</div>

// Or in className
<div className="bg-[var(--primary)] hover:bg-[var(--primary-hover)]">
  Element
</div>
```

## 🔄 Gradients

```tsx
<div className="bg-gradient-to-br from-[var(--background-gradient-from)] to-[var(--background-gradient-to)]">
  Gradient background
</div>
```

## 💡 Common Patterns

### Full Page Layout
```tsx
<div className="min-h-screen bg-gradient-to-br from-[var(--background-gradient-from)] to-[var(--background-gradient-to)]">
  <main className="bg-card text-card-foreground">
    Content
  </main>
</div>
```

### Form Input
```tsx
<input
  className="
    bg-card
    text-foreground
    border border-[var(--border)]
    hover:border-[var(--border-hover)]
    focus:border-[var(--border-focus)]
    focus:ring-2 focus:ring-[var(--border-focus)]
    placeholder:text-foreground-muted
    disabled:bg-disabled
    disabled:text-disabled-foreground
  "
/>
```

### Link
```tsx
<a className="text-accent hover:text-accent-hover hover:underline">
  Click here
</a>
```

### Navigation Link
```tsx
<a className="text-nav-link hover:text-nav-link-hover active:text-nav-link-active">
  Nav Item
</a>
```

## 🚫 Anti-Patterns (Don't Do This)

```tsx
// ❌ Hardcoded dark mode variants
<div className="bg-white dark:bg-gray-800">

// ❌ Specific Tailwind colors
<button className="bg-blue-600 hover:bg-blue-700">

// ❌ Manual color values
<div className="bg-[#ca8a04]">

// ❌ Inconsistent theming
<div className="text-stone-600 dark:text-stone-400">
```

## 🔧 Changing Theme Colors

1. Edit `src/app/globals.css`
2. Find the color in `:root` (light) or `.dark` (dark) section
3. Change the hex value
4. Save - changes apply instantly to entire site!

Example:
```css
:root {
  --primary: #your-new-color;
  --primary-hover: #your-hover-color;
}

.dark {
  --primary: #your-dark-mode-color;
  --primary-hover: #your-dark-hover-color;
}
```

## 📖 More Information

- Full theme schema: `docs/THEME_SCHEMA_FOR_DESIGNER.md`
- Theme configuration: `src/app/globals.css`
- Tailwind v4 docs: https://tailwindcss.com/docs

---

**Remember:** Always use theme tokens, never hardcode colors or dark mode variants!
