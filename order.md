1. Presentation
2. Claude Cowork
3. Obsidian
- Kanban Board
- Calendar view
- Create a task
4. Look at weekly, daily, and review
5. Go to last slide and questions
6. https://masontangnr.github.io/daily-brief/

Generate a Weekly Brief for my Obsidian vault. Save it as a new Markdown file named `weekly-[YYYY-MM-DD].md` (using today's date) inside the `Claude/weekly` folder of my Obsidian vault. The brief should have four sections:

## 1. Houston Events This Week

Search the web for events happening in Houston this week across these categories:

- Tech & AI meetups
- Business networking events
- Entrepreneurship / small business workshops
- Free online business classes or webinars
- General things to do (festivals, food events, outdoor activities)

List up to 40 items in a Markdown table with these columns: Event Name, Date/Time, Location, Category, and a one-sentence description. Sort by date. If a registration link is available, include it.

## 2. Houston Weather This Week

Search the web for the 7-day weather forecast for Houston, TX (Clear Lake area preferred). For each day, list:

- High / Low temperature (°F)
- Conditions (sunny, cloudy, rain, etc.)
- Any severe weather alerts

Present this as a simple Markdown table.

## 3. Weekly Task Review

Read all files in the `TaskNotes` folder of my Obsidian vault and extract any incomplete tasks (lines with `- [ ]`). Then:

- Group tasks by project or context (Studio Kairos, Clear Lake Tutors, Personal, etc.)
- Prioritize each task as 🔴 High, 🟡 Medium, or 🟢 Low based on deadlines and importance
- Estimate time for each task (e.g., ~30 min, ~2 hrs)
- For any complex or multi-step tasks, add a brief recommended approach (2–3 sentences on how to tackle it)

Format as grouped lists under H3 subheadings per project/context.

## 4. Chain Food Deals This Week

Search the web for current chain restaurant and fast food deals, coupons, and promotions available this week. Focus on:

- National chains with Houston locations (McDonald's, Burger King, Whataburger, Taco Bell, Chick-fil-A, Sonic, Freddy's, KFC, Blaze Pizza, Mod's Pizza, Jack in the Box, Cava  Chipotle, etc.)
- App-only deals and loyalty program offers
- Day-of-the-week specials (e.g., Taco Tuesday, Free Fry Friday)
- Limited-time promotions and seasonal menu deals
- Any notable coupon codes or promo codes

Present this as a Markdown table with these columns: Chain, Deal, Details/Conditions, and Days Available. Sort by chain name alphabetically. Note which deals require an app or loyalty membership.

---

**General formatting rules:**

- Use H2 (`##`) for each of the four main sections
- Use Obsidian-friendly Markdown (no HTML)
- Keep it scannable — favor tables and short bullet points over paragraphs
- Add a YAML frontmatter block at the top with `title`, `date`, and `tags: [weekly-brief]`

