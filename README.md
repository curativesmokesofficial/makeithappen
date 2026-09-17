# Gold Griffin OS - Final Moveable UserRoles

**Latest Build:** `GriffinOS_Dashboard.html` - No yellow box, no endpoint pills, IG Analyst cleaned, buttons don't show codes - only toast/status

**Fixes in this build (from screenshot image_7f8e42.png):**
- Removed big yellow box: "The Best Stack for You (free to start) - Use Replicate API - runs Luma Dream Machine / AnimateDiff"
- Removed small pill badges: ENDPOINT: POST /api/generate-animation and REPLICATE_API_TOKEN: missing
- Fixed IG Analyst section id='social-hub' - removed black code blocks POST /api/...
- Fixed clickable buttons to not show codes - Generate Animation/Mockup now show "Generating..." not code

**Architecture - Kept untouched:**
- Side menu: hamburger 44px z10082 clickable, drawer 280px z10081 slide, overlay z10080 display:none pointer-events:none
- UserRoles drag: ALL cards draggable handle ⋮⋮ top-left, HTML5 drag drop, touch, save layout localStorage, Move Mode toggle, resize both ↕↔
- id='design-studio' ONLY = Design Expert / Animation Generator Master Locks NEVER CHANGE
- id='commerce' ONLY = Clothing + Printful - Tee/Hoodie/Hat toggle useState mockupType, Drop Builder name/price/stock/releaseDate/designText, Preview loading, Generate Mockup /api/generate-mockup?type={mockupType}&text={designText}, Add to Drop, Publish Drop, 6-item grid
- id='social-hub' = IG Analyst - @curative_smokes 270 -5 Goal 500+ 54% top post Commercial Grow Supply warehouse tour 74 views
- id='settings' = REPLICATE_API_TOKEN + PRINTFUL_API_KEY type password save to localStorage, Test Connection

**Backend (hidden behind buttons, not shown in UI):**
- POST /api/generate-animation replicate.run('luma/dream-machine') with REPLICATE_API_TOKEN = localStorage.getItem('REPLICATE_API_TOKEN') || process.env.REPLICATE_API_TOKEN
- POST /api/generate-mockup Printful with PRINTFUL_API_KEY = localStorage.getItem('PRINTFUL_API_KEY') || process.env.PRINTFUL_API_KEY

**Files:**
- GriffinOS_Dashboard.html is_home
- base44_config.json branding #D4AF37 #0A4D2E #00D1FF #0A0E1A, integrations Google Drive, GitHub curative-smokes/designs, Instagram Graph @curative_smokes, Facebook 947927321956678, Adobe CC Photoshop Illustrator Premiere Pro, Asana
- base44_prompt.txt Master Locks, 4 Pillars Sacred Plant Education Behind-the-Scenes Buildouts Mindset/Free Soul Character Universe, Safety Monitor, Voice Workflow Hey Griffin assign trim to Juan and post grow tour Reel tomorrow 6pm -> Asana + file locator + safety check + queue Reel + Griffin Clippy Assigned queued safe Ready Commander?
