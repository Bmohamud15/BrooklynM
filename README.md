# BrooklynM
Remote Softball Coach
Here’s the full prompt. Copy and paste every word of this:

Build a single-page HTML website for a remote softball coaching business called Built by Brooklyn. The entire file must be one self-contained index.html with all CSS and JavaScript inside it. No external files. No frameworks. No npm. No images needed.

CRITICAL TECHNICAL RULES
∙ html and body must both have background-color: #0C1B33 set explicitly with !important
∙ Every single section must also explicitly set background-color — never rely on browser defaults
∙ All text must be light colored — never black, never dark gray
∙ No image tags anywhere. All package card headers use CSS gradient divs only.
∙ One file only: index.html. Pure HTML, CSS, JavaScript. Nothing else.
∙ Every “Book Your Session” button and every pricing button scrolls to #contact — no external links on any button

COLORS
∙ Dark navy (main background): #0C1B33
∙ Slightly lighter navy (alternate sections): #0a1628
∙ Darkest navy (footer): #060f1e
∙ Burnt orange (primary accent): #E8512A
∙ Cream (body text): #F5EFE4
∙ Gold (secondary accent): #C9A96E
∙ White: #FFFFFF

FONTS
Import from Google Fonts in the <head>:
https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&display=swap
∙ Headings: Bebas Neue
∙ Body: DM Sans

NAVIGATION
Fixed to top. Background rgba(12,27,51,0.88) with backdrop-filter: blur(14px). Bottom border 1px solid rgba(232,81,42,0.2). Padding 1.2rem 3rem.
Left side: text logo “BUILT BY BROOKLYN” in Bebas Neue, font-size 1.6rem, color #E8512A, no underline, links to # (top of page).
Right side: nav links in a flex row with 2.5rem gap. Links: About (href #about), Services (href #services), How It Works (href #how), Pricing (href #pricing). Font-size 0.85rem, uppercase, letter-spacing 0.12em, color #F5EFE4, opacity 0.75, no underline. Hover: opacity 1, color #E8512A.
Last nav item: filled orange button “Book Your Session” — background #E8512A, color white, padding 0.55rem 1.4rem, border-radius 2px. href is #contact. No external links. No new tab.
On mobile under 900px: hide all nav links, show only the logo.

HERO SECTION
Background #0C1B33. Two equal columns side by side. Min-height 100vh.
Left column — flex column, justify center, padding 9rem 4rem 6rem 3rem:
∙ Eyebrow line: font-size 0.75rem, letter-spacing 0.25em, uppercase, color #E8512A. Text: “Professional Remote Softball Coaching · All Levels”. Starts opacity 0, animates fadeUp with 0.2s delay.
∙ H1 in Bebas Neue, font-size clamp(4.5rem, 8vw, 8rem), line-height 0.92, color white. First line: “YOUR GAME.” Second line wrapped in a span colored #E8512A: “COACHED RIGHT.” Starts opacity 0, animates fadeUp with 0.4s delay.
∙ Paragraph body text font-size 1.05rem, line-height 1.7, color #F5EFE4, max-width 420px, margin-bottom 2.8rem. Text: “Film-based, position-specific coaching delivered to you — wherever you are. Send your video, get a plan, and start improving within days. No travel. No excuses. Just results.” Starts opacity 0, animates fadeUp with 0.6s delay.
∙ Two buttons side by side with 1rem gap, both fade up with 0.8s delay. Button 1: filled orange “Book Your Session” href #contact. Button 2: ghost outline “View Programs” href #services.
Right column — decorative graphic only, no images:
∙ Background linear-gradient(135deg, #142240 0%, #0C1B33 60%, #1a0c05 100%)
∙ Large circle 580x580px centered, border 1.5px solid rgba(232,81,42,0.15), slowly spinning 40s animation
∙ Inside circle: dashed inner circle border rgba(201,169,110,0.2)
∙ Diamond: 240x240px square rotated 45deg, border 2px solid rgba(232,81,42,0.4), centered
∙ Inner diamond inset 30px, border 1px solid rgba(201,169,110,0.3)
∙ Diagonal field lines at bottom using repeating-linear-gradient
∙ Badge bottom-right: background rgba(232,81,42,0.12), border 1px solid rgba(232,81,42,0.3), border-radius 4px, padding 1.2rem 1.6rem, text-align center, backdrop-filter blur 8px. Shows “100%” in Bebas Neue orange font-size 3rem and small label “Remote · Anywhere” below. Fades up with 1.2s delay.
On mobile: stack to single column, right column min-height 300px.

SCROLLING TICKER
Full-width bar, background #E8512A, overflow hidden, padding 0.7rem 0, white-space nowrap.
Inside: an inline-block div animating translateX(0) to translateX(-50%) over 22 seconds linearly and infinitely.
Items in Bebas Neue, font-size 1rem, letter-spacing 0.15em, color white, padding 0 2.5rem. Each item has ::after content ✦ opacity 0.6.
Items repeated twice for seamless loop: HITTING · INFIELD · OUTFIELD · CATCHING · GAME IQ · MENTAL GAME · VIDEO REVIEW · FILM ANALYSIS

ABOUT SECTION
id=“about”. Background #0C1B33. Border-top 1px solid rgba(255,255,255,0.06). Two columns, gap 6rem, align items center. Padding 7rem 3rem.
Left column — tall decorative card, aspect-ratio 4/5, background linear-gradient(160deg, #142240, #1a0c05), border-radius 4px, overflow hidden, position relative.
Inside: faint “BBK” text Bebas Neue font-size 14rem color rgba(232,81,42,0.08) absolute bottom-right. Vertical center line 2px rgba(201,169,110,0.12). At the bottom: 2x2 stat grid with 1px gaps, each cell background #0C1B33, padding 1.5rem, text-align center:
∙ “5+” / “Yrs Coaching”
∙ “100%” / “Remote Sessions”
∙ “All” / “Skill Levels”
∙ “Real” / “Results”
Stat numbers Bebas Neue font-size 2.8rem color #E8512A. Labels font-size 0.75rem uppercase letter-spacing 0.12em opacity 0.55.
Right column:
∙ Orange eyebrow “About Built by Brooklyn”
∙ Bebas Neue heading “COACHING WITH CONVICTION”
∙ Two cream body paragraphs: “Built by Brooklyn was built on one belief: great coaching shouldn’t be limited by where you live. With 5+ years of professional experience and a genuine passion for player development, we deliver position-specific instruction to athletes at every level — right through your screen.” and “From first-time players learning the basics to high school athletes chasing roster spots — every session is personalized, film-based, and built around you.”
∙ Filled orange button “Start Training →” margin-top 2.5rem, href #contact

SERVICES SECTION
id=“services”. Background #0a1628. Border-top 1px solid rgba(255,255,255,0.06). Padding 7rem 3rem.
Header: flex row space-between align flex-end margin-bottom 4rem. Left: eyebrow “What We Offer” + Bebas Neue heading “POSITION-FIRST DEVELOPMENT”. Right: cream paragraph max-width 340px: “Every area of the field coached with precision — film-reviewed, personalized, and built around how you actually play.”
2x2 grid of 4 cards, gap 1.5rem. Each card: background #0C1B33, border 1px solid rgba(255,255,255,0.06), border-radius 4px, padding 2.5rem 2rem, position relative, overflow hidden. Hover: border-color rgba(232,81,42,0.4), translateY -4px, subtle orange gradient overlay.
Card contents: large faint number Bebas Neue font-size 4rem color rgba(232,81,42,0.15), Bebas Neue title font-size 1.7rem white, cream description font-size 0.9rem opacity 0.65, small orange outlined tag font-size 0.7rem uppercase border 1px solid rgba(232,81,42,0.35) padding 0.3rem 0.75rem border-radius 2px margin-top 1.5rem.
4 cards:
1. 01 / HITTING / “Stance, load, swing path, bat speed, and situational hitting. We break down your swing frame by frame and rebuild it with purpose and confidence.” / tag: Video Analysis
2. 02 / INFIELD / “Footwork, fielding angles, glove work, hands, and throwing mechanics. Build the instincts and range that make you the anchor of your defense.” / tag: Position-Specific
3. 03 / OUTFIELD / “Drop steps, routes, fly ball reads, communication, and arm strength. Develop the skills to track down anything in the gap and make it look routine.” / tag: Film-Based Drills
4. 04 / CATCHING / “Framing, blocking, pop time, pitch calling, and field general skills. We develop catchers who control the game behind the plate and command the dugout.” / tag: Full Development

HOW IT WORKS SECTION
id=“how”. Background #0C1B33. Border-top 1px solid rgba(255,255,255,0.06). Padding 7rem 3rem.
Eyebrow “The Process” + Bebas Neue heading “HOW IT WORKS”.
One horizontal row of 4 connected boxes, margin-top 4rem. Container: border 1px solid rgba(255,255,255,0.06), border-radius 4px, overflow hidden, CSS grid 4 equal columns. Each step: padding 2.5rem 2rem, border-right 1px solid rgba(255,255,255,0.06), last one no border. Hover: background rgba(232,81,42,0.04). Position relative.
Between each step except last: small orange circle 1.4rem x 1.4rem, border-radius 50%, background #E8512A, position absolute top 2.5rem right -0.7rem, z-index 2, white “→” inside font-size 0.6rem.
Step contents: large faint Bebas Neue number font-size 5rem color rgba(232,81,42,0.18), Bebas Neue title 1.4rem white, cream description 0.87rem opacity 0.6.
4 steps:
1. BOOK A CALL — “Fill out the form below and we’ll reach out to learn your goals, skill level, and what you want to build. No commitment required.”
2. SEND YOUR FILM — “Record yourself hitting, fielding, or catching — phone camera is all you need. Upload and share before your first session.”
3. GET YOUR PLAN — “We build a custom training plan based on your film, goals, and schedule. Clear drills, clear benchmarks, clear path forward.”
4. TRAIN & GROW — “Live video sessions, ongoing film review, and consistent check-ins. Real coaching, real growth — all remote.”
On mobile: 2 columns instead of 4.

PRICING SECTION
id=“pricing”. Background #0a1628. Border-top 1px solid rgba(255,255,255,0.06). Padding 7rem 3rem.
Centered eyebrow “Packages” + centered Bebas Neue heading “FIND YOUR FIT”.
Three package cards in CSS grid 3 equal columns, gap 1.5rem, margin-top 4rem. Each card: border 1px solid rgba(255,255,255,0.08), border-radius 8px, background #0C1B33, overflow hidden, display flex, flex-direction column. Hover: translateY -5px.
Each card has a CSS gradient header div at the top — NO image tags. The header div has: width 100%, aspect-ratio 16/9, display flex, align-items center, justify-content center, border-radius 6px 6px 0 0, position relative, overflow hidden. Inside it: a span with the package name in Bebas Neue font-size 2rem letter-spacing 0.1em color white, text-shadow 0 2px 20px rgba(0,0,0,0.6), position relative z-index 1. The div also has a ::before pseudo-element with repeating-linear-gradient(45deg, transparent, transparent 20px, rgba(255,255,255,0.02) 20px, rgba(255,255,255,0.02) 21px) overlaid on top.
Card 1 gradient header: linear-gradient(135deg, #1a0c05 0%, #3d1a08 50%, #8B2500 100%). Text inside: “MAINTENANCE PACKAGE”
Card 2 gradient header: linear-gradient(135deg, #0C1B33 0%, #1a3a6b 50%, #E8512A 100%). Text inside: “STANDARD PACKAGE”
Card 3 gradient header: linear-gradient(135deg, #0a0a0a 0%, #2a1500 40%, #E8512A 100%). Text inside: “ELITE DEVELOPMENT”
Below the header div: a body div padding 1.8rem 1.8rem 2rem, flex 1, display flex, flex-direction column.
Body: gold tier label font-size 0.72rem letter-spacing 0.25em uppercase color #C9A96E, large Bebas Neue price font-size 3.5rem white line-height 1 with <sup>$</sup> before and /month after in small muted text, cream description font-size 0.87rem opacity 0.65 margin 0.8rem 0 1.2rem, bullet list no list-style each item has orange ✦ before it font-size 0.85rem opacity 0.75 padding 0.45rem 0 border-bottom 1px solid rgba(255,255,255,0.05), button at bottom margin-top auto.
Card 1 — MAINTENANCE / $200/month / “Stay sharp during the season or keep your mechanics fresh in the off-season.” / Bullets: Custom programming each month · Bi-weekly film review · Drill assignments between sessions · Responsive communication / Ghost outline button “Stay Sharp” href #contact
Card 2 — STANDARD / $300/month / Featured: orange border #E8512A, small orange badge top-right “Most Popular” background #E8512A font-size 0.65rem uppercase white padding 0.3rem 0.8rem border-radius 0 0 4px 4px position absolute / “Full development cycle with consistent programming, film-based feedback, and real results.” / Bullets: Custom monthly training plan · Weekly film analysis & feedback · Position-specific drill assignments · Ongoing communication & support / Filled orange button “Book Now” href #contact
Card 3 — ELITE DEVELOPMENT / $400/month / “The highest level of attention for the athlete who is fully committed to their development.” / Bullets: Comprehensive monthly programming · Full weekly film breakdowns · Game-day prep & strategy sessions · Priority response & scheduling · College recruiting guidance / Ghost outline button “Go Elite” href #contact
Below the 3 cards: wide horizontal assessment banner. Border 1px solid rgba(232,81,42,0.25), border-radius 8px, background #0C1B33, padding 2rem 2.5rem, display flex, gap 3rem, align-items center, margin-top 1.5rem. Hover: border-color #E8512A, translateY -3px.
Left side: orange eyebrow “Not sure where to start?”, Bebas Neue heading “SKILL ASSESSMENT” font-size 2rem white, cream description “Send us your film and we’ll evaluate your mechanics, identify the gaps, and give you a written breakdown with clear next steps.”, 3 inline bullet points with orange ✦: Full film review · Written breakdown report · Personalized recommendations.
Right side: Bebas Neue “$45” font-size 3.5rem white with orange <sup>$</sup>, small “one-time” label, filled orange button “Get Assessed” href #contact.
On mobile: 3 cards stack to 1 column, assessment banner stacks vertically.

TESTIMONIALS SECTION
id=“testimonials”. Background #0C1B33. Border-top 1px solid rgba(255,255,255,0.06). Padding 7rem 3rem.
Eyebrow “From Families We’ve Worked With” + Bebas Neue heading “REAL WORDS. REAL RESULTS.”
3 cards side by side, gap 1.5rem, margin-top 4rem. Each card: background #0d1e38, border 1px solid rgba(255,255,255,0.06), border-radius 4px, padding 2rem. Hover: border-color rgba(232,81,42,0.25).
Each card: 5 orange stars ★★★★★ font-size 0.75rem letter-spacing 0.1em. Large faint quote mark Bebas Neue font-size 4rem color #E8512A opacity 0.4 line-height 0.8. Italic cream testimonial text font-size 0.95rem line-height 1.75 opacity 0.8 margin-bottom 1.5rem. Bold white author name font-size 0.9rem. Small muted role label font-size 0.75rem opacity 0.5.
3 real testimonials:
1. “Thank you for all you did for Paisley. She hasn’t had very many coaches believe in her and really care to develop her. You made a huge impact on her and I’m forever grateful.” — Paisley’s Mom · Parent · Built by Brooklyn Athlete
2. “She learned so much and has gained so much more confidence since working with you. We appreciate your patience and support with Jerzi. She’s beyond happy and so proud of herself.” — Jerzi’s Mom · Parent · Built by Brooklyn Athlete
3. “You are the best thing that happened to Bristol. She has improved so much.” — Bristol’s Family · Parent · Built by Brooklyn Athlete
On mobile: stack to 1 column.

CONTACT SECTION
id=“contact”. Background #E8512A. Padding 7rem 3rem. Two columns gap 6rem align items center.
Left column:
∙ Eyebrow color rgba(255,255,255,0.6): “Get In Touch”
∙ Bebas Neue heading color white: “LET’S BUILD YOUR GAME”
∙ White body text opacity 0.75: “Ready to take your game to the next level? Fill out the form and we’ll be in touch within 24 hours.”
∙ Info lines margin-top 1.5rem white opacity 0.75: “📍 Remote — Available Nationwide” and “📱 Sessions via Zoom, FaceTime, or Google Meet”
Right column — contact form with these fields, all stacked:
∙ Row: First Name + Last Name side by side
∙ Email (full width)
∙ Row: Player Age + Primary Focus dropdown (options: Hitting, Infield, Outfield, Catching, Full Game)
∙ Goals textarea full width min-height 110px
∙ Question textarea full width min-height 80px with label “Any questions?”
∙ Submit button: background #0C1B33, color white, padding 1rem 2.5rem, DM Sans font-size 0.85rem font-weight 500 uppercase letter-spacing 0.12em, text “Send My Info →”
All inputs/select/textarea: background rgba(255,255,255,0.12), border 1px solid rgba(255,255,255,0.25), border-radius 2px, padding 0.8rem 1rem, color white, DM Sans. Placeholder color rgba(255,255,255,0.35). Focus border-color white. Select options background #0C1B33. Form labels: font-size 0.72rem uppercase letter-spacing 0.18em color rgba(255,255,255,0.6).
On submit: validate that First Name and Email are not empty. If either is empty show an alert saying “Please enter your first name and email.” If valid: use window.location.href to open a mailto link that sends to builtbybrooklyn@gmail.com. The mailto subject should be “New Coaching Inquiry – Built by Brooklyn”. The mailto body should include all 6 fields: First Name, Last Name, Email, Player Age, Primary Focus, Goals, and Question, each on its own line labeled clearly. After triggering the mailto, hide the form div and show a success div with background rgba(255,255,255,0.15), border 1px solid rgba(255,255,255,0.4), border-radius 4px, padding 1.5rem, centered white text, Bebas Neue heading “YOU’RE IN! 🎉” font-size 1.8rem, and subtext “Thanks for reaching out! We’ll be in touch within 24 hours.”
On mobile: stack to 1 column.

FOOTER
Background #060f1e. Padding 3rem. Flex row space-between align center flex-wrap wrap gap 1.5rem. Border-top 1px solid rgba(255,255,255,0.05).
Left: “BUILT BY BROOKLYN” Bebas Neue 1.4rem color #E8512A.
Center: links — About (#about), Services (#services), Pricing (#pricing), Contact (#contact). Font-size 0.8rem color #F5EFE4 opacity 0.4 no underline. Hover opacity 0.9.
Right: “© 2026 Built by Brooklyn. All rights reserved.” font-size 0.75rem opacity 0.3.
On mobile: flex-direction column text-align center.

ALL ANIMATIONS
∙ fadeUp: from opacity:0; transform:translateY(24px) to opacity:1; transform:translateY(0). All animated elements start with opacity:0 and use animation-fill-mode: forwards.
∙ spin: hero circle rotates 0 to 360deg over 40s linear infinite, kept centered with translate(-50%,-50%).
∙ ticker: moves from translateX(0) to translateX(-50%) over 22s linear infinite.
∙ Hover transitions on cards: transition: transform 0.25s, border-color 0.25s.

FINAL CHECKLIST
∙ html { background-color: #0C1B33 !important; scroll-behavior: smooth; }
∙ body { background-color: #0C1B33 !important; color: #F5EFE4; }
∙ Every section has an explicit background-color in CSS
∙ Zero image tags in the entire file
∙ Zero links to forms.gle anywhere
∙ Every button either scrolls to #contact or is the submit button
∙ The mailto goes to builtbybrooklyn@gmail.com
∙ File is named index.html
∙ No external JavaScript libraries
∙ Fully responsive at 900px breakpoint​​​​​​​​​​​​​​​​
