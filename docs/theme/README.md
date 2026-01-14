# 🎨 Theme System Overview

The VulcanoConnects theme system provides a comprehensive set of design tokens that ensure visual consistency across the entire platform.

## 🌟 Key Features

- **70+ Design Tokens** - Complete coverage of colors, typography, spacing, and more
- **Light & Dark Modes** - Automatic theme switching with proper contrast
- **Tailwind CSS v4** - Modern utility-first CSS framework
- **Type-Safe** - TypeScript definitions for all tokens
- **Designer-Friendly** - Clear schema for design handoff

## 📁 Documentation Files

| File | Audience | Purpose |
|------|----------|---------|
| [designer-schema.md](designer-schema.md) | Designers | Complete token reference with usage guidelines |
| [developer-guide.md](developer-guide.md) | Developers | Code examples and implementation patterns |
| [migration-status.md](migration-status.md) | Team | Track implementation progress |

## 🎯 Theme Categories

### Colors
- **Brand Colors**: Primary, Secondary, Accent
- **State Colors**: Success, Error, Warning, Info
- **UI Colors**: Backgrounds, Foregrounds, Borders
- **Interactive States**: Hover, Focus, Active, Disabled

### Typography
- **Font Families**: Display, Body, Code
- **Font Sizes**: From xs (0.75rem) to 5xl (3rem)
- **Font Weights**: 400 (normal) to 700 (bold)
- **Line Heights**: Optimized for readability

### Layout
- **Spacing Scale**: Consistent rhythm (0.25rem increments)
- **Border Radius**: From subtle (0.25rem) to pill (9999px)
- **Shadows**: Elevation system for depth

## 🚀 Quick Start for Designers

1. **Review the [Designer Schema](designer-schema.md)** - This is your complete reference
2. **Understand token naming** - Semantic names (e.g., `primary`, `error`) not descriptive (e.g., `yellow`, `red`)
3. **Design for both themes** - Always specify light AND dark mode values
4. **Use the color system** - Never use arbitrary colors; all colors should map to tokens

## 🛠️ Quick Start for Developers

1. **Review the [Developer Guide](developer-guide.md)** - Learn how to use tokens in code
2. **Use theme classes** - `bg-primary`, `text-foreground`, etc.
3. **Avoid hardcoded colors** - Always use theme tokens
4. **Test both themes** - Verify appearance in light and dark modes

## 💡 Design Principles

### Consistency
Every color, spacing, and typography choice should use a theme token. This ensures:
- Visual consistency across the platform
- Easy theme updates (change once, apply everywhere)
- Accessibility (proper contrast ratios)

### Semantic Naming
Tokens use semantic names that describe their purpose, not their appearance:
- ✅ `--primary` (describes purpose)
- ❌ `--yellow-600` (describes appearance)

This allows the underlying color to change without breaking the semantic meaning.

### Dark Mode First
The theme system treats light and dark modes as equal citizens:
- Both are fully specified
- Proper contrast ratios for accessibility
- Consistent component appearance across themes

## 📊 Implementation Status

Check [migration-status.md](migration-status.md) for current implementation progress across the codebase.

---

## 🤝 Contributing to the Theme

If you're proposing theme changes:
1. Update the [designer-schema.md](designer-schema.md) with new tokens
2. Ensure both light and dark values are specified
3. Maintain accessibility standards (WCAG 2.1 AA minimum)
4. Document usage examples in [developer-guide.md](developer-guide.md)
