# LinkedInsight Style Guide

## Brand Overview
LinkedInsight features a clean, minimalist design system with strong black & white contrast, distinctive shadow effects, and a professional monospace aesthetic.

## 🎨 Color Palette

### Light Theme
- **Primary Background**: `#FFFFFF` / `hsl(0, 0%, 100%)`
- **Secondary Background**: `#F5F5F5` / `hsl(0, 0%, 96.1%)`
- **Tertiary Background**: `#EDEDED` / `hsl(0, 0%, 93%)`
- **Window Background**: `rgb(237, 237, 237)`

- **Primary Text**: `#0A0A0A` / `hsl(0, 0%, 3.9%)`
- **Secondary Text**: `#737373` / `hsl(0, 0%, 45.1%)`
- **Tertiary Text**: `#A6A6A6` / `hsl(0, 0%, 65%)`

- **Primary Border**: `#000000` / `hsl(0, 0%, 0%)`
- **Subtle Border**: `#E5E5E5` / `hsl(0, 0%, 89.8%)`

- **Button Primary**: Background `#000000`, Text `#FFFFFF`
- **Button Secondary**: Background `#F5F5F5`, Text `#0A0A0A`

### Dark Theme
- **Primary Background**: `#0A0A0A` / `hsl(0, 0%, 3.9%)`
- **Secondary Background**: `#262626` / `hsl(0, 0%, 14.9%)`
- **Tertiary Background**: `#1A1A1A` / `hsl(0, 0%, 10%)`
- **Window Background**: `hsl(0, 0%, 3.9%)`

- **Primary Text**: `#FAFAFA` / `hsl(0, 0%, 98%)`
- **Secondary Text**: `#A3A3A3` / `hsl(0, 0%, 63.9%)`
- **Tertiary Text**: `#737373` / `hsl(0, 0%, 45%)`

- **Primary Border**: `#FFFFFF` / `hsl(0, 0%, 100%)`
- **Subtle Border**: `#262626` / `hsl(0, 0%, 14.9%)`

- **Button Primary**: Background `#FFFFFF`, Text `#000000`
- **Button Secondary**: Background `#4D4D4D`, Text `#FAFAFA`

### Accent Colors
- **Error**: Light `hsl(0, 100%, 95%)`, Dark `hsl(0, 100%, 15%)`
- **Error Text**: Light `hsl(0, 100%, 30%)`, Dark `hsl(0, 100%, 70%)`

## 📐 Typography

### Font Families
- **Base Font**: `Arial, Helvetica, sans-serif`
- **Heading Font**: `'Archivo', sans-serif` (Google Font)
- **Monospace Font**: `'IBM Plex Mono', monospace` (Google Font)

### Font Weights
- Regular: 400
- Medium: 500
- Bold: 700

### Font Sizes (Component Classes)
- **Form Title**: `1.5rem` (24px)
- **Body Text**: `1rem` (16px)
- **Small Text**: `0.875rem` (14px)
- **Extra Small**: `0.75rem` (12px)
- **Headings**: 
  - H1: `2xl` (1.5rem/24px)
  - H2: `xl` (1.25rem/20px)
  - H3: `lg` (1.125rem/18px)

## 🎯 Key Design Patterns

### Border Radius
- **Small**: `0.25rem` (4px)
- **Medium**: `0.375rem` (6px)
- **Large**: `0.5rem` (8px)

### Shadows
- **Signature Shadow**: `7px 7px 0px 0px` with color:
  - Light: `hsl(0, 0%, 30%)`
  - Dark: `hsl(0, 0%, 27%)`
- **Shadow Offset**: `7px` (used for margin calculations)

### Spacing System
- **space-1**: `0.25rem` (4px)
- **space-2**: `0.5rem` (8px)
- **space-3**: `0.75rem` (12px)
- **space-4**: `1rem` (16px)
- **space-5**: `1.25rem` (20px)
- **space-6**: `1.5rem` (24px)
- **space-8**: `2rem` (32px)
- **space-10**: `2.5rem` (40px)
- **space-11**: `2.75rem` (44px)
- **space-12**: `3rem` (48px)

## ✨ Animations & Transitions

### Transition Durations
- **Fast**: `150ms ease`
- **Normal**: `250ms ease`
- **Slow**: `350ms ease`

### Easing Functions
- **Ease Out**: `cubic-bezier(0.25, 0.8, 0.25, 1)`
- **Ease In**: `cubic-bezier(0.55, 0, 1, 0.45)`
- **Ease In Out**: `cubic-bezier(0.4, 0, 0.2, 1)`

### Common Animations
1. **Page Transitions**
   - Entry: Fade in + slide up (300ms)
   - Exit: Fade out + slide up (250ms)

2. **Pulse Propagation**
   - Linear wave effect across elements
   - 3s duration with 1.5s delay between waves

3. **Loading Spinner**
   - 360° rotation
   - 0.75s - 1s duration

4. **Fade In**
   - Simple opacity animation
   - 0.3s ease-in-out

## 🖼️ Brand Assets

### Logo Files
- **Main Icon**: `/public/STORYD_Icon_Black.png`
- **Favicon**: `/public/favicon_small.png`
- **Logo**: `/public/logo.png`

## 🎨 Distinctive Features

1. **Shadow Containers**: Signature 7px offset shadow boxes with black borders
2. **Monospace Aesthetic**: Heavy use of IBM Plex Mono for UI elements
3. **High Contrast**: Strong black/white contrast in both themes
4. **Dot Grid Background**: Subtle dot pattern (20px grid) on body
5. **Non-resizable Textareas**: Fixed-size input areas for consistency
6. **Grayscale Emojis**: Filtered to maintain monochrome aesthetic

## 💻 Implementation Notes

### CSS Variables
All design tokens are defined as CSS custom properties in `:root` and `[data-theme="dark"]`

### Theme Switching
- Supports light/dark/system themes
- Uses `data-theme` attribute on document root
- Stores preference in localStorage

### Component Classes
Pre-built component classes available:
- `.shadow-container` - Signature shadow box
- `.button-primary/secondary` - Styled buttons
- `.textarea-input` - Styled textareas
- `.form-container` - Form layouts
- `.loading-spinner` - Loading states

### Responsive Design
- Container max-width: 1400px (2xl screens)
- Mobile-first approach with Tailwind breakpoints