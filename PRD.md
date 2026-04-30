# **📄 Product Requirements Document (PRD)**

## **Interactive Portfolio – p5.js Projects**

---

## **1\. Overview**

**Product Name:** p5.js Interactive Portfolio  
 **Owner:** Alan Horvat

**Purpose:**  
 Build a visually engaging portfolio website to showcase **11 interactive p5.js sketches**, allowing users to **experience** each project directly in the browser rather than just viewing static descriptions.

**Core Idea:**  
 This is not just a portfolio—it’s a **playable gallery**.

---

## **2\. Goals**

* Showcase all 11 projects as **interactive experiences**  
* Let users **run and interact** with each sketch instantly  
* Demonstrate creativity, coding ability, and experimentation  
* Create a memorable, unique portfolio (not generic)  
  ---

  ## **3\. Target Users**

  ### **Primary**

* Recruiters (frontend / creative coding / UI roles)

  ### **Secondary**

* Professors / evaluators

  ### **User Expectations**

* “Show me what this does” (not just read)  
* Fast interaction (no setup required)  
* Clear explanation of concept \+ code  
  ---

  ## **4\. Product Vision**

A **gallery-style website** where:

* Each project is a **live canvas**  
* Users can **interact immediately**  
* Projects feel like **mini digital artworks**  
  ---

  ## **5\. Key Features**

  ---

  ### **5.1 Homepage (Gallery Entry)**

**Purpose:** Immediate visual impact

**Features:**

* Grid of 11 project thumbnails (animated previews if possible)  
* Hover → quick interaction or preview  
* Click → opens project experience

**Content:**

* Title (your name)  
* Short tagline (e.g., “Interactive Experiments with p5.js”)  
  ---

  ### **5.2 Project Experience Page (Core Feature)**

**This is the most important part.**

**Each project page includes:**

#### **🎮 Live Canvas**

* Embedded p5.js sketch (auto-run)  
* Fully interactive (mouse, keyboard, etc.)

  #### **🧾 Info Panel**

* Title  
* Short description (what it does)  
* Concept / idea  
* Controls (e.g., “Move mouse to change color”)

  #### **🛠 Tech Details**

* Tools used (p5.js, JS)  
* Link to GitHub

  #### **🔁 Reset Button**

* Restart sketch if needed  
  ---

  ### **5.3 Navigation**

* Next / Previous project buttons  
* Back to gallery  
* Keyboard navigation (optional but impressive)  
  ---

  ### **5.4 About Section**

* Short bio  
* What you explored in these projects:  
  * Generative art  
  * Interaction design  
  * Animation  
* Skills list  
  ---

  ## **6\. Functional Requirements**

* All 11 sketches must:  
  * Load correctly  
  * Run smoothly in browser  
* No page reload needed between interactions (preferred)  
* Responsive layout (desktop priority, mobile acceptable)  
  ---

  ## **7\. Non-Functional Requirements**

* Performance:  
  * Sketch loads \< 2 seconds  
* Stability:  
  * No crashes/freezing sketches  
* Usability:  
  * Clear instructions for interaction

  ---

  ## **8\. Design Requirements**

**Style Direction:**

* Minimal UI → focus on artwork  
* Dark mode preferred (better for visuals)  
* Clean typography

**Layout Concept:**

* Fullscreen canvas for projects  
* Overlay UI for text  
  ---

  ## **9\. Information Architecture**

  Home (Gallery)  
    ├── Project 1 (Interactive)  
    ├── Project 2  
    ├── ...  
    └── Project 11  
  About  
  ---

  ## **10\. Tech Stack (Recommended)**

* **Core:** HTML, CSS, JavaScript  
* **Library:** p5.js  
* **Optional Framework:** React or Next.js (if comfortable)

**Hosting:**

* GitHub Pages  
* Vercel / Netlify  
  ---

  ## **11\. Content Requirements**

For each of the 11 projects, prepare:

* Title  
* 1–2 sentence description  
* Interaction instructions  
* Screenshot (fallback)  
* GitHub link  
  ---

  ## **12\. Timeline (Fast Build Plan)**

**Week 1**

* Setup structure  
* Build gallery page

**Week 2**

* Integrate 5–6 sketches

**Week 3**

* Add remaining sketches  
* Add project info panels

**Week 4**

* Polish UI  
* Optimize performance  
* Deploy  
  ---

  ## **13\. Success Metrics**

* All 11 projects are interactive and working  
* Users can understand each project in \< 10 seconds  
* Portfolio feels unique vs standard portfolios  
* Ready to send to recruiters  
  ---

  ## **14\. Risks & Mitigation**

| Risk | Mitigation |
| ----- | ----- |
| Sketch performance issues | Optimize draw loops |
| Too chaotic visually | Keep UI minimal |
| User confusion | Add clear interaction instructions |

  ---

  ## **15\. Future Enhancements**

* Add sound-based interactions  
* Add project filters (e.g., “Generative”, “Game”)  
* Add fullscreen mode toggle  
* Add “random project” button  
  ---

  ## **💡 Key Advice (important)**

If you treat this like a normal portfolio, it will feel **boring**.

Lean into what makes p5.js special:

* motion  
* interactivity  
* surprise

