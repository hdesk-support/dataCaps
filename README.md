📋 Data Capture Form
Overview
The Data Capture Form is a single‑file, offline‑first web application built entirely in index.html. It is designed for customer care and product tracking, with responsive layouts, accessibility features, and dynamic record management—all without external dependencies.

✨ Features
Offline‑first storage Records are saved in the browser’s local storage, ensuring functionality even without internet access.

Dynamic UI controls
Theme toggle (light, dark, high‑contrast).
Font scaling (increase, decrease, reset).

Record management
Save, view, edit, and clear records.
Duplicate detection modal to prevent repeated entries.
Inline editing of stored records.

Accessibility & responsiveness
Semantic HTML5 structure.
Keyboard‑friendly focus rings.
Layout adapts across mobile, tablet, and desktop.

Guided onboarding
Built‑in guide cards and reminder lists.

Storage quota tracking
Progress bar with color‑coded usage levels (low, medium, high).

Dynamic dropdowns
Dependent select fields (e.g., reasons → sub‑reasons) defined directly in the HTML/JS.
Logic ensures child options update automatically when a parent option changes.

🛠️ How It Works
Single‑file structure
All HTML, CSS, and JavaScript are embedded in index.html.
No external assets or folders are required.

UI rendering
The header provides theme/font controls and record actions.
The main form and guide sections are revealed when triggered.
Modals handle record viewing, duplicates, and form input.

Data capture & storage
Form inputs are validated and stored locally.
Records can be viewed, edited inline, or cleared entirely.

Dropdown logic
Parent/child relationships (e.g., reasons → sub‑reasons) are coded directly in the <select> elements and supporting JavaScript blocks inside index.html.
Editing these sections updates the available options for users.

📂 Maintenance Guide
Since this is a single‑file app, all updates happen inside index.html. Maintainers should focus on:

Dropdowns and dependent logic
Locate <select> elements for reasons, sub‑reasons, and categories.
Update <option> values or adjust the JavaScript mappings nearby.
Ensure consistency between parent and child dropdowns.
Record management logic
Review the modal sections (#recordsModal, #duplicatesModal) for table structures.
Inline editing and duplicate detection are handled in the embedded JS.

UI controls
Theme toggles, font scaling, and accessibility features are defined in the header and supporting script blocks.
Adjust variables in the :root CSS section for color or typography changes.
Storage quota bar
Progress bar styles and thresholds are defined in the CSS and updated via JS logic.
Modify labels or thresholds directly in the relevant section.
