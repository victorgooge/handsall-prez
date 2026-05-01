# Zoku All-Hands Presentation - Build Specification

## Project Overview
Build a single-file HTML presentation with horizontal drag/swipe navigation for Zoku's first monthly all-hands meeting on May 1, 2026. The presentation should be visually stunning with smooth animations, modern design, and work perfectly in fullscreen mode.

## Technical Requirements

### File Structure
- Single `zoku-presentation.html` file
- All CSS inline in `<style>` tag
- All JavaScript inline in `<script>` tag
- Load external dependencies from CDN only:
  - Google Fonts: Inter or Plus Jakarta Sans
  - GSAP (GreenSock Animation Platform): https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/gsap.min.js
  - Font Awesome icons (optional): https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css

### Browser Support
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Fullscreen mode support (F11 or Fn+F on presentation)
- Responsive design (works on any screen size)

## Design Specifications

### Color Palette
```css
/* Background */
--bg-primary: #0f0f1e; /* Deep navy/charcoal */
--bg-secondary: #1a1a2e; /* Slightly lighter */
--bg-card: rgba(255, 255, 255, 0.05); /* Glassmorphism base */

/* Gradients (for accents) */
--gradient-purple: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
--gradient-pink: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
--gradient-blue: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
--gradient-green: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
--gradient-sunset: linear-gradient(135deg, #fa709a 0%, #fee140 100%);
--gradient-ocean: linear-gradient(135deg, #30cfd0 0%, #330867 100%);
--gradient-soft: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);

/* Text */
--text-primary: #ffffff;
--text-secondary: rgba(255, 255, 255, 0.7);
--text-tertiary: rgba(255, 255, 255, 0.5);
```

### Typography
```css
font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
/* Alternative: 'Plus Jakarta Sans' */

/* Sizes */
--text-hero: 72px;
--text-title: 48px;
--text-subtitle: 32px;
--text-body: 20px;
--text-small: 16px;
```

### Glassmorphism Card Style
```css
background: rgba(255, 255, 255, 0.05);
backdrop-filter: blur(10px);
border: 1px solid rgba(255, 255, 255, 0.1);
border-radius: 20px;
box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
```

## Slide Structure (7 slides total)

Each slide is a full viewport panel. Use placeholder content marked with `[TBD]` for sections that will be filled in later.

### Slide 1: Opening / Hero
```
Content:
- Zoku logo/wordmark (large, centered)
- Event title: "Zoku All-Hands Meeting"
- Date: "Friday, May 1, 2026"
- Time: "5:30 PM"
- Animated entrance: Logo fades in, then title slides up, then date/time stagger in
- Background: Animated gradient mesh or particle effect (subtle)

Design notes:
- Centered layout
- Large hero text
- Gradient accent on title
```

### Slide 2: Company Updates
```
Content:
- Section title: "Company Updates"
- Subtitle: "Where Zoku stands today"
- 3-4 glassmorphism cards with key metrics/updates:
  * Card 1: "[TBD - Overall progress metric]"
  * Card 2: "[TBD - Growth/traction metric]"
  * Card 3: "[TBD - Platform status]"
  * Card 4: "[TBD - User engagement]"
- Each card has an icon, number/stat, and label

Animation:
- Title slides in from left
- Cards stagger in from bottom with 100ms delay between each
```

### Slide 3: Key Milestones
```
Content:
- Section title: "Key Milestones"
- Subtitle: "What we've achieved"
- Timeline or list of achievements:
  * "[TBD - Major milestone 1]"
  * "[TBD - Major milestone 2]"
  * "[TBD - Major milestone 3]"
  * "[TBD - Major milestone 4]"
- Use icons or checkmarks for visual interest
- Display as vertical timeline or card grid

Animation:
- Timeline items fade in sequentially from top to bottom
```

### Slide 4: Frontend Team Update
```
Content:
- Section title: "Frontend Team Update"
- Subtitle: "What we've been building"
- Content sections (in glassmorphism cards):
  
  ### What we worked on:
  - "[TBD - Feature/project 1]"
  - "[TBD - Feature/project 2]"
  - "[TBD - Feature/project 3]"
  
  ### Key accomplishments:
  - "[TBD - Win 1]"
  - "[TBD - Win 2]"
  
  ### Current projects:
  - "[TBD - Ongoing work 1]"
  - "[TBD - Ongoing work 2]"
  
  ### Timeline & goals:
  - "[TBD - Next sprint goal]"
  - "[TBD - Month goal]"

Design notes:
- Two-column layout or card grid
- Icons for each section
- This is the main slide that will be heavily customized

Animation:
- Section headers slide in from left
- Content fades in with stagger
```

### Slide 5: Timeline & Status
```
Content:
- Section title: "Timeline & Project Status"
- Subtitle: "Current status across all teams"
- Project status board or timeline:
  * Backend Team: "[TBD - Status/progress]"
  * Frontend Team: "[TBD - Status/progress]"
  * Design Team: "[TBD - Status/progress]"
  * Mobile Team: "[TBD - Status/progress]"
- Use progress bars or status badges (In Progress, Completed, Planned)
- Visual timeline showing Q2-Q3-Q4 2026

Animation:
- Progress bars animate from 0 to target percentage
- Timeline items fade in left to right
```

### Slide 6: Next Steps
```
Content:
- Section title: "Next Steps"
- Subtitle: "Priorities for V2"
- List of priorities (numbered or bulleted):
  1. "[TBD - Priority 1]"
  2. "[TBD - Priority 2]"
  3. "[TBD - Priority 3]"
  4. "[TBD - Priority 4]"
- Roadmap visual showing path to V2 launch
- Target date: "[TBD - V2 launch target]"

Animation:
- Items slide in from right with stagger
- Roadmap path draws in with SVG line animation
```

### Slide 7: Team & Closing
```
Content:
- Section title: "The Team"
- Grid of team member cards (placeholders):
  * Name: "[Team Member Name]"
  * Role: "[Role]"
  * Avatar placeholder (colored circle with initials)
- Shoutouts section: "[TBD - Recognition/kudos]"
- Closing message: "Questions?" or "Let's build Zoku V2!"
- Footer: "Thank you • Zoku Team • May 2026"

Animation:
- Team cards fade in with stagger grid animation
- Closing message pulses or has subtle glow effect
```

## Navigation Mechanics

### Horizontal Slide Navigation
```javascript
// Implement smooth horizontal scrolling between slides
// Each slide is 100vw wide
// Container is flex row with scroll-snap

Features required:
1. Mouse drag to navigate
   - Click and drag left/right
   - Momentum scrolling with easing
   - Snap to nearest slide on release

2. Touch/swipe support
   - Touch drag on mobile/tablet
   - Swipe gestures
   - Momentum and snap

3. Keyboard controls
   - Arrow Left: previous slide
   - Arrow Right: next slide
   - Home: first slide
   - End: last slide
   - Escape: exit fullscreen

4. Dot navigation
   - Bottom-center indicator dots
   - Show current slide (highlighted)
   - Click any dot to jump to that slide
   - Smooth scroll transition

5. Smooth transitions
   - 600ms ease-in-out transition
   - No jarring jumps
   - Respect prefers-reduced-motion
```

### Slide Entry Animations
```javascript
// When entering a slide, trigger stagger animations on content
// Use GSAP or CSS animations
// Elements should have data-animate attribute

Animation sequence per slide:
1. Detect slide becomes visible
2. Find all [data-animate] elements
3. Stagger animate them in (opacity 0→1, translateY 30px→0)
4. 100ms delay between each element
5. Total stagger duration ~800ms
```

## Responsive Behavior

```css
/* Desktop (default) */
font-size: base

/* Tablet (< 1024px) */
- Reduce font sizes by 15%
- Adjust card grid to 2 columns max

/* Mobile (< 768px) */
- Single column layouts
- Reduce font sizes by 25%
- Larger touch targets for navigation
- Dots navigation slightly larger
```

## Performance Requirements

- 60fps animations (no jank)
- Smooth drag/scroll on all devices
- Fast initial load (< 1 second)
- No layout shift during animations
- GPU-accelerated transforms (use transform/opacity for animations, not position/width/height)

## Code Quality

- Well-commented code sections
- Clear variable names
- Modular JavaScript functions
- Semantic HTML structure
- Accessible (keyboard navigation, ARIA labels where needed)

## Deployment Instructions

Include at the top of the HTML file as a comment:

```html
<!--
ZOKU ALL-HANDS PRESENTATION
Created: [Date]
Event: Friday, May 1, 2026, 5:30 PM

DEPLOYMENT INSTRUCTIONS:

Option 1: Netlify Drop (Recommended - 10 seconds)
1. Go to: https://app.netlify.com/drop
2. Drag this HTML file into the browser window
3. Netlify will give you an instant URL like: amazing-tesla-abc123.netlify.app
4. Share that URL with your team
5. Present from the URL in fullscreen (F11 or Fn+F)

Option 2: GitHub Pages
1. Create a new GitHub repo
2. Upload this file as "index.html"
3. Go to Settings → Pages → Enable Pages
4. Your URL will be: yourusername.github.io/repo-name

Option 3: Vercel
1. Go to vercel.com
2. Drag this file to deploy
3. Instant URL provided

Option 4: Share the file directly
1. Zip the HTML file: zoku-presentation.zip
2. Share via email/Slack
3. Recipients: Unzip → Open in browser

PRESENTING:
- Open the URL or file in Chrome/Firefox/Safari
- Press F11 (or Fn+F on Mac) for fullscreen
- Use arrow keys ← → to navigate
- Or drag/swipe left/right
- Click dots at bottom to jump to slides
- Press Esc to exit fullscreen

CUSTOMIZATION:
- Search for "[TBD]" to find all placeholder content
- Replace placeholders with actual data
- Adjust colors in CSS variables if needed
- Add/remove slides by duplicating slide sections
-->
```

## Final Checklist

Before considering the build complete, verify:

- [ ] All 7 slides are present and properly structured
- [ ] Horizontal drag navigation works smoothly
- [ ] Keyboard arrow keys work
- [ ] Dot navigation indicators work and show current slide
- [ ] Touch/swipe works on mobile
- [ ] All animations are smooth (60fps)
- [ ] Glassmorphism cards render correctly
- [ ] Fonts load from Google Fonts
- [ ] File is self-contained (no external dependencies except CDN)
- [ ] Deployment instructions are in HTML comment
- [ ] All placeholder content is marked with [TBD]
- [ ] Responsive design works on mobile/tablet/desktop
- [ ] Fullscreen mode works (F11)
- [ ] No console errors

## Example Card Component

```html
<div class="glass-card" data-animate>
  <div class="card-icon">
    <i class="fas fa-rocket"></i>
  </div>
  <div class="card-stat">
    [TBD - Number/Metric]
  </div>
  <div class="card-label">
    [TBD - Label/Description]
  </div>
</div>
```

## Notes for Claude Code

- This is a presentation for a startup's all-hands meeting
- Prioritize visual polish and smooth animations
- The horizontal slider navigation is critical - it should feel premium
- Use GSAP for animations if confident, otherwise pure CSS is fine
- Make it look professional but modern (not corporate boring)
- Glassmorphism should be subtle, not overdone
- Dark background is essential for the aesthetic
- All placeholder content will be filled in later by the user
- The file should be production-ready except for placeholder content
