# Theme Configuration Schema for Designer

This document lists ALL theme tokens that need to be defined for both light and dark themes. Please provide color values (hex codes) and font specifications for each item.

## How to Use This Document

1. For each token, provide the value for **Light Theme** and **Dark Theme**
2. Colors should be in hex format (e.g., `#FFFFFF`)
3. Font sizes use `rem` units (e.g., `1rem` = 16px)
4. Font weights are numeric (400 = normal, 500 = medium, 600 = semibold, 700 = bold)

---

## 🎨 BACKGROUND COLORS

### Page Backgrounds
| Token | Description | Light Theme | Dark Theme |
|-------|-------------|-------------|------------|
| `--background` | Main page background | `#ffffff` | `#0a0a0a` |
| `--background-gradient-from` | Gradient start color | `#fafaf9` | `#18181b` |
| `--background-gradient-to` | Gradient end color | `#f5f5f4` | `#27272a` |

---

## 📝 TEXT COLORS (Foregrounds)

### Primary Text
| Token | Description | Light Theme | Dark Theme |
|-------|-------------|-------------|------------|
| `--foreground` | Main body text | `#232323` | `#fafafa` |
| `--foreground-secondary` | Secondary text (less emphasis) | `#57534e` | `#a1a1aa` |
| `--foreground-muted` | Muted text (subtle) | `#78716c` | `#71717a` |

---

## 🃏 CARDS & SURFACES

### Card Elements
| Token | Description | Light Theme | Dark Theme |
|-------|-------------|-------------|------------|
| `--card` | Card background | `#ffffff` | `#18181b` |
| `--card-foreground` | Text on cards | `#232323` | `#fafafa` |
| `--card-hover` | Card background on hover | `#fafafa` | `#27272a` |

---

## 🎯 BRAND COLORS

### Primary Brand Color (Main CTAs, highlights)
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--primary` | Primary brand color | `#ca8a04` | `#eab308` | Main buttons, links |
| `--primary-hover` | Primary hover state | `#a16207` | `#fbbf24` | Button hover |
| `--primary-foreground` | Text on primary | `#ffffff` | `#18181b` | Button text |
| `--primary-light` | Primary tint/background | `#fef9c3` | `#713f12` | Subtle highlights |

### Secondary Brand Color (Supporting elements)
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--secondary` | Secondary brand color | `#57534e` | `#52525b` | Secondary buttons |
| `--secondary-hover` | Secondary hover state | `#44403c` | `#71717a` | Button hover |
| `--secondary-foreground` | Text on secondary | `#ffffff` | `#fafafa` | Button text |
| `--secondary-light` | Secondary tint | `#f5f5f4` | `#27272a` | Subtle backgrounds |

### Accent Color (Links, highlights)
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--accent` | Accent color | `#2563eb` | `#3b82f6` | Links, badges |
| `--accent-hover` | Accent hover state | `#1d4ed8` | `#60a5fa` | Link hover |
| `--accent-foreground` | Text on accent | `#ffffff` | `#ffffff` | Badge text |
| `--accent-light` | Accent tint | `#dbeafe` | `#1e3a8a` | Subtle accents |

---

## ✅ STATE COLORS

### Success States
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--success` | Success color | `#16a34a` | `#22c55e` | Success messages |
| `--success-hover` | Success hover | `#15803d` | `#4ade80` | Success button hover |
| `--success-foreground` | Text on success | `#ffffff` | `#ffffff` | Success text |
| `--success-light` | Success tint | `#dcfce7` | `#14532d` | Success backgrounds |

### Error/Danger States
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--error` | Error color | `#dc2626` | `#ef4444` | Error messages |
| `--error-hover` | Error hover | `#b91c1c` | `#f87171` | Error button hover |
| `--error-foreground` | Text on error | `#ffffff` | `#ffffff` | Error text |
| `--error-light` | Error tint | `#fee2e2` | `#7f1d1d` | Error backgrounds |

### Warning States
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--warning` | Warning color | `#ea580c` | `#f97316` | Warning messages |
| `--warning-hover` | Warning hover | `#c2410c` | `#fb923c` | Warning button hover |
| `--warning-foreground` | Text on warning | `#ffffff` | `#ffffff` | Warning text |
| `--warning-light` | Warning tint | `#ffedd5` | `#7c2d12` | Warning backgrounds |

---

## 🔲 BORDERS

### Border Colors
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--border` | Default border | `#e7e5e4` | `#3f3f46` | All borders |
| `--border-hover` | Border on hover | `#d6d3d1` | `#52525b` | Interactive borders |
| `--border-focus` | Border on focus | `#ca8a04` | `#eab308` | Form inputs focus |

---

## 🔇 MUTED/SUBTLE ELEMENTS

### Muted Colors
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--muted` | Muted background | `#f5f5f4` | `#27272a` | Subtle backgrounds |
| `--muted-foreground` | Muted text | `#78716c` | `#71717a` | Helper text |

---

## 🚫 DISABLED STATES

### Disabled Elements
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--disabled` | Disabled background | `#d6d3d1` | `#3f3f46` | Disabled buttons |
| `--disabled-foreground` | Disabled text | `#a8a29e` | `#52525b` | Disabled text |

---

## 🧭 NAVIGATION

### Navigation Bar
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--nav-background` | Nav bar background | `#ffffff` | `#18181b` | Header background |
| `--nav-foreground` | Nav bar text | `#232323` | `#fafafa` | Header text |
| `--nav-border` | Nav bar border | `#e7e5e4` | `#3f3f46` | Header border |
| `--nav-link` | Nav link color | `#57534e` | `#a1a1aa` | Link color |
| `--nav-link-hover` | Nav link hover | `#ca8a04` | `#eab308` | Link hover |
| `--nav-link-active` | Active nav link | `#a16207` | `#fbbf24` | Active link |

---

## 🦶 FOOTER

### Footer Section
| Token | Description | Light Theme | Dark Theme | Usage |
|-------|-------------|-------------|------------|-------|
| `--footer-background` | Footer background | `#ffffff` | `#18181b` | Footer background |
| `--footer-foreground` | Footer text | `#232323` | `#fafafa` | Footer text |
| `--footer-border` | Footer border | `#e7e5e4` | `#3f3f46` | Footer top border |
| `--footer-link` | Footer link color | `#57534e` | `#a1a1aa` | Footer links |
| `--footer-link-hover` | Footer link hover | `#ca8a04` | `#eab308` | Footer link hover |

---

## 🔤 TYPOGRAPHY

### Font Sizes
| Token | Description | Current Value | Designer Value |
|-------|-------------|---------------|----------------|
| `--font-size-xs` | Extra small text | `0.75rem` (12px) | |
| `--font-size-sm` | Small text | `0.875rem` (14px) | |
| `--font-size-base` | Base/body text | `1rem` (16px) | |
| `--font-size-lg` | Large text | `1.125rem` (18px) | |
| `--font-size-xl` | Extra large | `1.25rem` (20px) | |
| `--font-size-2xl` | Heading 4 | `1.5rem` (24px) | |
| `--font-size-3xl` | Heading 3 | `1.875rem` (30px) | |
| `--font-size-4xl` | Heading 2 | `2.25rem` (36px) | |

### Font Weights
| Token | Description | Current Value | Designer Value |
|-------|-------------|---------------|----------------|
| `--font-weight-normal` | Normal text | `400` | |
| `--font-weight-medium` | Medium emphasis | `500` | |
| `--font-weight-semibold` | Semibold | `600` | |
| `--font-weight-bold` | Bold text | `700` | |
| `--font-weight-extrabold` | Extra bold | `800` | |

### Line Heights
| Token | Description | Current Value | Designer Value |
|-------|-------------|---------------|----------------|
| `--line-height-tight` | Tight (headings) | `1.25` | |
| `--line-height-normal` | Normal (body) | `1.5` | |
| `--line-height-relaxed` | Relaxed | `1.75` | |

### Font Families
| Token | Description | Current Value | Designer Value |
|-------|-------------|---------------|----------------|
| `--font-family-sans` | Body font | Inter, system-ui | |
| `--font-family-logo` | Logo/heading font | Orbitron | |

---

## 📏 SPACING

### Standard Spacing Scale
| Token | Description | Current Value | Designer Value |
|-------|-------------|---------------|----------------|
| `--spacing-xs` | Extra small | `0.25rem` (4px) | |
| `--spacing-sm` | Small | `0.5rem` (8px) | |
| `--spacing-md` | Medium | `1rem` (16px) | |
| `--spacing-lg` | Large | `1.5rem` (24px) | |
| `--spacing-xl` | Extra large | `2rem` (32px) | |
| `--spacing-2xl` | 2x large | `3rem` (48px) | |

---

## 🔘 BORDER RADIUS

### Corner Rounding
| Token | Description | Current Value | Designer Value |
|-------|-------------|---------------|----------------|
| `--radius-sm` | Small radius | `0.375rem` (6px) | |
| `--radius-md` | Medium radius | `0.5rem` (8px) | |
| `--radius-lg` | Large radius | `0.75rem` (12px) | |
| `--radius-xl` | Extra large | `1rem` (16px) | |
| `--radius-full` | Fully rounded | `9999px` | |

---

## 🌑 SHADOWS

### Box Shadows (Auto-calculated per theme)
| Token | Description | Usage |
|-------|-------------|-------|
| `--shadow-sm` | Small shadow | Subtle elevation |
| `--shadow-md` | Medium shadow | Cards, dropdowns |
| `--shadow-lg` | Large shadow | Modals, popovers |

---

## 📋 USAGE GUIDE

### Component Mapping

**Buttons:**
- Primary CTA → `--primary` / `--primary-hover` / `--primary-foreground`
- Secondary action → `--secondary` / `--secondary-hover` / `--secondary-foreground`
- Success → `--success` / `--success-hover` / `--success-foreground`
- Danger → `--error` / `--error-hover` / `--error-foreground`

**Links:**
- Default → `--accent`
- Hover → `--accent-hover`

**Forms:**
- Border → `--border`
- Focus border → `--border-focus`
- Background → `--card`
- Text → `--foreground`
- Placeholder → `--foreground-muted`

**Messages:**
- Success → `--success-light` background, `--success` border/icon
- Error → `--error-light` background, `--error` border/icon
- Warning → `--warning-light` background, `--warning` border/icon

---

## 🚀 Implementation Notes

1. All values are defined in `src/app/globals.css`
2. Changes to this file automatically update the entire site
3. Use Tailwind v4 custom color classes: `bg-primary`, `text-foreground`, etc.
4. For one-off colors, use: `bg-[var(--primary)]`
5. Dark mode automatically switches when user toggles theme

---

**Last Updated:** January 14, 2026
**Tailwind Version:** 4.1.18
**Designer:** [TO BE FILLED]
