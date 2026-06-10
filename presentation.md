**Title:** Build an AI-Powered time management system using Claude Cowork and Obsidian

**Description:** Stop spending your Mondays figuring out your priorities and Fridays wondering what you accomplished for the week. In this session, you'll learn how to combine Claude Cowork's scheduled automation with Obsidian's flexible note system to generate daily briefs, weekly briefs, and weekly reviews, all on autopilot. Whether you're a entrepreneur or just someone who wants to start each day with clarity, this presentation will show you how to make AI do the boring planning work so you can focus on the real work.

---

**Slide Outline:**

**Slide 1 — Title Slide** Presentation title, your name
**Slide 2 — About Me** Information about Studio Kairos, Clear Lake Tutors and being an educator for 15 years
**Slide 3 — Topic** The presentation is for anyone who wants to an AI powered system to organize their business, work or personal life.
- Obsidian
- Claude Cowork
- Daily Briefs, Weekly Briefs, and Weekly Review
**Slide 4   — The Problem** Most people start their week without a plan and end it without a reflecting on their week which results in poor time management.
- What tasks should I do today?
- What is priority for each task?
- What is the time estimate for each task?
- When should I complete the task and in which order?
- Did I use my time efficiently this week and how can I improve in the future?
**Slide 5 — Obsidian**
- Free Note Taking application
- Uses Markdown files on your computer
- Open Source Plugin to download
	- TaskNote Pluggin
		- It has calendar, kanban board, create tasks, task list all in one.
**Slide 6 — Claude Cowork
- AI Desktop App that can create files on your computer
- Schedule- make edits on your computer with time and can be recurring
- Create daily briefs, presentations,  reports, automate file organizations, and generate spreadsheets.
**Slide 7 — System Architecture
- Visual diagram showing the three automations, their schedules, and how they flow into the Obsidian vault folder structure (`Claude/daily`, `Claude/weekly`, `Claude/reviews`).
**Slide 8 — Weekly Brief 
- Houston events this week
- Houston weather this week
- Weekly tasks review
	- Group tasks by project or context
	- Prioritize each task as 🔴 High, 🟡 Medium, or 🟢 Low based on deadlines and importance
	- Time Estimate for each task
	- For any complex tasks, add a brief recommended approach (2–3 sentences on how to tackle it)
- Coupons for fast food restaurant
**Slide 9 — Weekly Brief Prompt
- Generate a Weekly Brief for my Obsidian vault. Save it as a new Markdown file named `weekly-[YYYY-MM-DD].md` (using today's date) inside the `Claude/weekly` folder of my Obsidian vault. The brief should have four sections: ## 1. Houston Events This Week Search the web for events happening in Houston this week across these categories: - Tech & AI meetups - Business networking events - Entrepreneurship / small business workshops - Free online business classes or webinars - General things to do (festivals, food events, outdoor activities) List up to 40 items in a Markdown table with these columns: Event Name, Date/Time, Location, Category, and a one-sentence description. Sort by date. If a registration link is available, include it. ## 2. Houston Weather This Week Search the web for the 7-day weather forecast for Houston, TX (Clear Lake area preferred). For each day, list: - High / Low temperature (°F) - Conditions (sunny, cloudy, rain, etc.) - Any severe weather alerts Present this as a simple Markdown table. ## 3. Weekly Task Review Read all files in the `TaskNotes` folder of my Obsidian vault and extract any incomplete tasks (lines with `- [ ]`). Then: - Group tasks by project or context (Studio Kairos, Clear Lake Tutors, Personal, etc.) - Prioritize each task as 🔴 High, 🟡 Medium, or 🟢 Low based on deadlines and importance - Estimate time for each task (e.g., ~30 min, ~2 hrs) - For any complex or multi-step tasks, add a brief recommended approach (2–3 sentences on how to tackle it) Format as grouped lists under H3 subheadings per project/context. ## 4. Chain Food Deals This Week Search the web for current chain restaurant and fast food deals, coupons, and promotions available this week. Focus on: - National chains with Houston locations (McDonald's, Burger King, Whataburger, Taco Bell, Chick-fil-A, Sonic, Freddy's, KFC, Blaze Pizza, Mod's Pizza, Jack in the Box, Cava Chipotle, etc.) - App-only deals and loyalty program offers - Day-of-the-week specials (e.g., Taco Tuesday, Free Fry Friday) - Limited-time promotions and seasonal menu deals - Any notable coupon codes or promo codes Present this as a Markdown table with these columns: Chain, Deal, Details/Conditions, and Days Available. Sort by chain name alphabetically. Note which deals require an app or loyalty membership. --- **General formatting rules:** - Use H2 (`##`) for each of the four main sections - Use Obsidian-friendly Markdown (no HTML) - Keep it scannable — favor tables and short bullet points over paragraphs - Add a YAML frontmatter block at the top with `title`, `date`, and `tags: [weekly-brief]`
**Slide 10 — Daily Brief 
- Houston Weather for today
- Weekly Task Review
- Today Focus
	- Pick top 3- 5 task
	- Arrange them into time blocks
	- Give each task priority
	- For complex tasks, add a brief recommendation approach
**Slide 11 — Daily Brief 
- Generate a Daily Brief for my Obsidian vault. Save it as a new Markdown file named `daily-[YYYY-MM-DD].md` (using today's date) inside the `Claude/daily` folder of my Obsidian vault. The brief should have three sections: ## 1. Weekly Task Review Read all files in the `TaskNotes` folder of my Obsidian vault and extract any incomplete tasks (lines with `- [ ]`). Then: - Group tasks by project or context (Studio Kairos, Clear Lake Tutors, Personal, etc.) - Prioritize each task as 🔴 High, 🟡 Medium, or 🟢 Low based on deadlines and importance - Estimate time for each task (e.g., ~30 min, ~2 hrs) - For any complex or multi-step tasks, add a brief recommended approach (2–3 sentences on how to tackle it) Format as grouped lists under H3 subheadings per project/context. - Only put tasks for this week and Not for future weeks ## 2. Today's Focus Based on the weekly task review above, build a focused daily plan for today: - Pick the top 3–5 tasks I should realistically tackle today, considering priority and time estimates - Arrange them into a suggested schedule with time blocks (morning, midday, afternoon, evening) - Flag any tasks that are blocked or depend on someone else - If the day looks overloaded, recommend what to defer and why Format as a numbered list with time blocks and brief reasoning for each pick. General formatting rules: - Use H2 (`##`) for each of the three main sections - Use Obsidian-friendly Markdown (no HTML) - Keep it scannable — favor short bullet points over paragraphs - Add a YAML frontmatter block at the top: yaml ```yaml --- title: "Daily Brief — [YYYY-MM-DD]" date: [YYYY-MM-DD] tags: [daily-brief] type: daily-note --- ```
**Slide 12 — Weekly Review 
- Completed tasks this week
- Wins this week
	- Note top 3-5 meaning full progress and describe why it was important
- Areas for improvement
- Lessons Learned
- Open Task Carried Forward
- Next Week's Priorities
**Slide 13 — Weekly Review Prompt
- Generate a Weekly Review for my Obsidian vault. Save it as a new Markdown file named `review-[YYYY-MM-DD].md` (using today's date) inside the `Claude/weekly-review` folder of my Obsidian vault. ## 1. Completed Tasks This Week Read all files in the `TaskNotes` folder of my Obsidian vault and extract any tasks that were completed this week (lines with `- [x]`). Then: - Group by project or context (Studio Kairos, Clear Lake Tutors, Personal, etc.) - For each group, list the completed tasks - Add a task count per group and a total count at the end Format as grouped lists under H3 subheadings per project/context. ## 2. Wins This Week Based on the completed tasks above, identify 3–5 notable wins — things that moved the needle, unblocked something important, or represent meaningful progress. For each win: - Describe what was accomplished in one sentence - Explain why it matters — what it unlocked, what goal it advances, or what problem it solved - Suggest momentum actions — one small next step to keep the progress going Format as a numbered list. ## 3. Areas for Improvement Analyze the week honestly and identify 3–5 areas for improvement. Consider: - Tasks that were carried over from previous weeks and still aren't done — why are they stuck? - Tasks that took longer than expected — what caused the drag? - Gaps in focus — was time spent on the right priorities, or did low-value work eat the week? - Patterns — recurring blockers, procrastination triggers, or workflow friction worth addressing For each area: - Name the issue clearly - Identify the root cause (not just the symptom) - Suggest a specific, actionable change for next week Format as a numbered list. ## 4. Lessons Learned Capture 3–5 reusable insights from this week — things worth remembering beyond just this review. These can come from wins, failures, surprises, or anything in between. Consider: - Technical lessons — a tool, workflow, or code approach that worked well (or didn't) that's worth documenting - Business lessons — something learned about clients, pricing, sales, or running the businesses - Teaching lessons — insights from tutoring sessions about how students learn, what materials land, or what doesn't work - Personal productivity lessons — discoveries about how you work best, what drains energy, or what creates flow For each lesson: - State the lesson as a clear, memorable one-liner (something you could re-read in 6 months and immediately understand) - Add context — what happened that surfaced this lesson - Tag it with a category: `#technical`, `#business`, `#teaching`, or `#productivity` Format as a numbered list. These should be written as durable insights — not task-specific notes, but principles or patterns you'd want your future self to remember. ## 5. Open Tasks Carried Forward List all remaining incomplete tasks (lines with `- [ ]`) that are carrying into next week: - Group by project or context - Flag any that are overdue or have been open for more than two weeks - For flagged items, recommend whether to prioritize, delegate, renegotiate the deadline, or drop Format as grouped lists under H3 subheadings per project/context. ## 6. Next Week's Priorities Based on everything above, recommend the top 5 priorities for next week, considering: - Unfinished high-priority work carried forward - Momentum from this week's wins worth continuing - Improvement areas that need deliberate attention - Any lessons learned that suggest a change in approach For each priority, include a one-sentence rationale. Format as a numbered list. General formatting rules: - Use H2 (`##`) for each of the six main sections - Use Obsidian-friendly Markdown (no HTML) - Keep it scannable — favor short bullet points over paragraphs - Be honest and constructive in the improvement section — direct but not harsh - Add a YAML frontmatter block at the top: yaml ```yaml --- title: "Weekly Review — [YYYY-MM-DD]" date: [YYYY-MM-DD] tags: [weekly-review] type: weekly-note --- ```
**Slide 14 — Contact
- Website- clearlaketutor.com
- email- clearlaketutoring@gmail.com
- linkedIn- https://www.linkedin.com/in/mason-tang-87696b65/
- presentation URL- TBD
 