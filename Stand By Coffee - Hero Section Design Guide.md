# Stand By Coffee - Hero Section Design Guide
## Video Background Strategy

---

## **LAYOUT STRUCTURE**

### **Video Background Setup**
- **Overlay**: Dark semi-transparent overlay (rgba(0,0,0,0.5) to 0.6) to dim the video and ensure text readability
- **Video Properties**:
  - Fixed position, full viewport coverage
  - Autoplay, muted, loop
  - Object-fit: cover (maintains aspect ratio)
  - z-index: -1 (stays behind content)

---

## **CONTENT PLACEMENT & ALIGNMENT**

### **Option 1: LEFT-ALIGNED (Recommended for this video)**
```
┌─────────────────────────────────────┐
│ STAND BY                            │
│ COFFEE                              │
│                                     │
│ Your Daily Escape                   │
│ Premium coffee & delicious bites    │
│ in the heart of Worli               │
│                                     │
│ [Explore Menu]  [Reserve Table]     │
│                                     │
│ ⭐ 4.1★ | 358+ Reviews | Open 7:30AM│
└─────────────────────────────────────┘
```
- **Logo/Brand**: Top-left corner (60px from top, 40px from left)
- **Main Headline**: Left side, 20% from top
- **Subheadline**: Left side, below headline
- **Description**: Left side, 2-3 lines max
- **CTA Buttons**: Left side, below description
- **Stats**: Bottom-left corner

**Why Left-Aligned?** The video has warm café interior on the left side - text placement here creates visual balance and doesn't compete with the focal points in the video.

---

### **Option 2: CENTER-ALIGNED (Alternative)**
- Everything centered vertically & horizontally
- Works if you want a more dramatic, bold approach
- Risk: Text might overlap with important video elements

---

## **TYPOGRAPHY & TEXT STYLING**

### **Logo/Brand Name**
- Font: Bold, sans-serif (e.g., Montserrat, Poppins Bold)
- Size: 24-32px
- Color: **White** (#FFFFFF)
- Letter-spacing: 2px (for elegance)
- Position: Top-left, fixed

### **Main Headline** ("Your Daily Escape")
- Font: Serif, elegant (e.g., Playfair Display, Georgia)
- Size: 56-72px (desktop), 36-48px (mobile)
- Color: **White** (#FFFFFF)
- Font-weight: 700 (bold)
- Line-height: 1.2
- Text-shadow: 2px 2px 8px rgba(0,0,0,0.7) ← **CRITICAL for readability**

### **Subheadline** ("Premium coffee & delicious bites...")
- Font: Regular sans-serif (e.g., Open Sans, Inter)
- Size: 18-24px (desktop), 14-16px (mobile)
- Color: **Light gray/off-white** (#E8E8E4 or #D0D0D0)
- Font-weight: 400 (regular)
- Line-height: 1.6
- Max-width: 500px (prevents long lines)
- Text-shadow: 1px 1px 4px rgba(0,0,0,0.6)

### **CTA Buttons**
- **Primary Button** ("Explore Menu"):
  - Background: Gradient (from #C28B6C to #8B6F47) - warm terracotta
  - Text: White, bold
  - Padding: 14px 32px
  - Border-radius: 8px
  - Font-size: 16px
  - Hover: Slight scale (1.05) + glow effect

- **Secondary Button** ("Reserve Table"):
  - Background: Transparent with white border (2px)
  - Text: White
  - Padding: 14px 32px
  - Border-radius: 8px
  - Hover: Background becomes rgba(255,255,255,0.1)

### **Stats Section**
- Font: Bold sans-serif
- Size: 14-16px
- Color: White
- Layout: Flex row with dividers (|)
- Example: "⭐ 4.1★ | 358+ Reviews | Open 7:30 AM"

---

## **SPACING & POSITIONING**

### **Desktop Layout (1024px+)**
```
Top Padding: 120px (from top of viewport)
Left Padding: 60px (from left edge)
Content Width: 500px max
Line Spacing: 24px between elements
Button Gap: 16px
```

### **Tablet Layout (768px - 1023px)**
```
Top Padding: 100px
Left Padding: 40px
Content Width: 450px max
Font sizes: Reduce by 10-15%
```

### **Mobile Layout (< 768px)**
```
Top Padding: 80px
Left Padding: 24px
Right Padding: 24px
Content Width: 100% - 48px
Font sizes: Reduce by 20-25%
Buttons: Stack vertically (full width)
```

---

## **COLOR PALETTE FOR VIDEO BG**

Since the video has warm, moody café tones (browns, golds, warm blacks):

- **Text**: White (#FFFFFF) - maximum contrast
- **Accent Text**: Light cream (#F5F5DC) - for secondary info
- **Button Primary**: Warm terracotta (#C28B6C) - complements video
- **Button Secondary**: Transparent white border
- **Overlay**: Dark semi-transparent (rgba(0,0,0,0.55))

---

## **VISUAL HIERARCHY**

1. **Logo** (smallest, top-left)
2. **Main Headline** (largest, most prominent)
3. **Subheadline** (medium, secondary)
4. **CTA Buttons** (action-focused)
5. **Stats** (supporting info, bottom)

---

## **ANIMATION & MICRO-INTERACTIONS**

### **On Page Load**
- Logo: Fade in + slide down (300ms)
- Headline: Fade in + slide up (400ms, 100ms delay)
- Subheadline: Fade in + slide up (400ms, 200ms delay)
- Buttons: Fade in + scale (400ms, 300ms delay)
- Stats: Fade in (500ms, 400ms delay)

### **Hover Effects**
- **Buttons**: Scale 1.05 + subtle shadow
- **Stats**: Slight color change on hover

### **Scroll Effects**
- Content fades out as user scrolls (parallax effect optional)
- Video continues playing in background

---

## **OVERLAY STRATEGY**

### **Why Dim the Video?**
- Ensures text is readable
- Creates depth and focus
- Prevents video from competing with content

### **Overlay Options**
1. **Solid Dark Overlay**: `rgba(0,0,0,0.55)` - Simple, effective
2. **Gradient Overlay**: 
   ```
   linear-gradient(135deg, 
     rgba(0,0,0,0.7) 0%, 
     rgba(0,0,0,0.4) 50%, 
     rgba(0,0,0,0.6) 100%)
   ```
   - Creates visual interest
   - Darker on left (where text is) for better readability

3. **Vignette Overlay** (advanced):
   - Darker edges, lighter center
   - Draws focus to the middle

---

## **RESPONSIVE BREAKPOINTS**

| Breakpoint | Layout | Font Sizes | Buttons |
|-----------|--------|-----------|---------|
| 1920px+ | Left-aligned, full spacing | 72px headline | Side-by-side |
| 1024px | Left-aligned, standard | 56px headline | Side-by-side |
| 768px | Left-aligned, reduced | 42px headline | Side-by-side |
| 480px | Left-aligned, compact | 32px headline | Stacked |
| < 480px | Centered, minimal | 28px headline | Stacked, full-width |

---

## **ACCESSIBILITY CONSIDERATIONS**

- **Text Contrast**: Ensure WCAG AA compliance (4.5:1 ratio for body text)
- **Text-shadow**: Improves readability on video backgrounds
- **Font-size**: Minimum 16px for body text
- **Button Size**: Minimum 44x44px for touch targets
- **Keyboard Navigation**: All buttons accessible via Tab key
- **Prefers-reduced-motion**: Disable animations for users who prefer it

---

## **FINAL CHECKLIST**

- ✅ Video background set to fixed, cover, muted, loop
- ✅ Overlay applied (0.55 opacity dark layer)
- ✅ Logo positioned top-left
- ✅ Headline left-aligned, white, with text-shadow
- ✅ Subheadline readable, max-width 500px
- ✅ CTA buttons styled with hover effects
- ✅ Stats section at bottom-left
- ✅ Mobile responsive layout tested
- ✅ Text contrast meets WCAG standards
- ✅ Animations smooth and purposeful

---

## **IMPLEMENTATION PRIORITY**

1. **Phase 1**: Video background + overlay + basic text layout
2. **Phase 2**: Styling (colors, fonts, shadows)
3. **Phase 3**: Buttons and interactions
4. **Phase 4**: Animations and micro-interactions
5. **Phase 5**: Mobile responsiveness refinement
