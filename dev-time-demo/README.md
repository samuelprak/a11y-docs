I'm preparing an interactive presentation about web accessibility for our dev team
the goal: show them a website, and let they find accessibility issues.
Like, i'm displaying a blurred checklist, and once someone reveals an issue I check it and explain
would it work? wdyt? what should i show to them, the most popular accessibility mistakes?

Your idea is **excellent**! Making accessibility training interactive—like a live audit game—will engage the dev team and help them internalize key issues.

## Why Your Format Works

- **Interactivity:** People learn best by doing. Spotting issues themselves is more memorable than a lecture.
- **Checklist Reveal:** The blurred checklist adds a game-like element (think “bingo” or “treasure hunt”), making the session fun and competitive.
- **Immediate Explanation:** When an issue is revealed, you can explain why it matters—building empathy for real users.

---

## How to Do It

### 1. **Choose a Website**
- Use your own product (if possible), or a known site with issues.
- Or, create a purposefully “broken” demo page with common accessibility mistakes built in.

### 2. **Prepare Your Checklist**
- Make a list of **top accessibility issues** (see below).
- Blur or hide the list on your slide.
- Unblur/check items as the team finds them.

### 3. **Guide the Team**
- Let them explore the site in pairs or groups.
- Encourage using both mouse and keyboard.
- Optionally, let them try a screen reader (Mac: VoiceOver; Windows: NVDA).

### 4. **Celebrate Discoveries**
- When someone finds an issue, reveal it on the checklist.
- Explain *what* the issue is, *why* it matters, and *how* to fix it.

---

## What to Include: The Most Common Accessibility Issues

Here’s a ready-to-use checklist of the most frequent (and teachable) accessibility mistakes:

### **The Classic Accessibility Issues**
1. **Missing or poor alt text** on images
2. **Low color contrast** between text and background
3. **No keyboard navigation** (can’t tab through links/buttons)
4. **Non-semantic HTML** (using `<div>`/`<span>` instead of headings, lists, etc.)
5. **Missing form labels** or unassociated labels
6. **No visible focus indicator** for interactive elements
7. **Links/buttons without accessible names** ("click here" or icon-only with no label)
8. **Improper heading structure** (skipping levels, not using `<h1>`, etc.)
9. **Content that’s only visible on hover** (not accessible for keyboard or screen reader users)
10. **No skip link** to bypass navigation

---

## Optional: Tools to Help

- **axe DevTools** (browser extension)
- **Wave Evaluation Tool**
- **Browser’s built-in accessibility inspector**

Let your team try these after the “manual” phase—showing how tools can help, but can’t catch everything.

---

## Bonus: Tips for Success

- **Timebox** the hunt (e.g., 10–15 min) to keep energy high.
- **Make it safe**—remind everyone it’s about learning, not blame.
- **Wrap up** with key takeaways and practical next steps for your team.

---

**Summary:**  
Your approach is effective and fun. Focus on the most common and high-impact issues, use real examples, and foster discussion. If you want, I can help you make the blurred checklist, sample slides, or a demo site full of accessibility “traps.” Let me know what you need!

---


Let's build a DoctoStore - A web page where Doctolib employees can buy goodies (mugs, stickers, etc.). About CSS, make it simple, nice and professional.
No fancy animations, no fancy effects, no fancy transitions, no fancy anything, just simple, nice and professional.
We'll build a single page with the following accessibility issues:

- Missing or poor alt text on images (one image with missing alt, and one decorative image with useless alt)
- Low color contrast between text and background (a button/text behind background?)
- No keyboard navigation (can’t tab through links/buttons)
- Non-semantic HTML (using <div>/<span> instead of headings, lists, etc.)
- Missing form labels or unassociated labels (could be a mailing list signup form?)
- No visible focus indicator for interactive elements
- Links/buttons without accessible names ("click here" or icon-only with no label)- 
- Improper heading structure (skipping levels, not using <h1>, etc.)
- Content that’s only visible on hover (not accessible for keyboard or screen reader users)
- No skip link to bypass navigation

DoctoStore - Doctolib Employee Store
│
├── Header Navigation
│   ├── Logo (image without alt text)
│   ├── Search Input (unlabeled)
│   ├── Search Icon Button (div styled as button, no accessible name, icon-only)
│   ├── Account Menu (hover-only dropdown)
│   └── Cart Icon (no accessible name)
│
├── Hero Section (small and simple)
│   ├── Welcome Message at the left (low contrast text)
│   ├── Banner Image at the right (decorative with useless alt text, e.g. "two men walking and holding goodies")
│   └── "Shop Now" Button (poor focus indicator)
│
├── Product Categories (left sidebar) (non-semantic divs instead of lists)
│   ├── Mugs & Drinkware
│   ├── Apparel & Accessories  
│   ├── Tech Gadgets
│   └── Office Supplies
│
├── Featured Products Grid (main content)
│   ├── Product Cards (missing headings structure)
│   │   ├── Product Image (missing alt text)
│   │   ├── Product Name (span instead of heading)
│   │   ├── Price (low contrast)
│   │   └── "Add to Cart" (generic button text)
│   │
│   └── Product Quick View (hover-only details)
│
└── Footer
    ├── Company Links (generic "click here" links)
    ├── Social Media Icons (no labels)
    └── Copyright (span instead of semantic footer)
