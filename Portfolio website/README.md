Student Name: Elizabeth Ngungu
Student ID: [2510462201]
GitHub Repository: [Your Repository URL]

# HTML Personal Portfolio Website

## Question 1: Website Creation

I built a **personal portfolio website** for myself as a Software Engineering student and aspiring web/cyber security developer based in Lusaka, Zambia. The site is built using only HTML (no external CSS or JavaScript) and is organized into clear, semantic sections:

- **Header** – my name, title/tagline, and a navigation bar linking to every section.
- **About Me** – a short bio, my profile photo, and a quote about learning to program.
- **Skills** – a bulleted list of technical skills (Python, HTML, CSS, JavaScript, VS Code) and a numbered list of security/soft skills, plus a collapsible `<details>` block listing the tools I use.
- **Projects** – a table listing my projects (Safemode: Firewall v0.1, Cyber Firewall Website, HTML Portfolio Website) with their description, tech stack, and status, along with a link to my GitHub.
- **Education** – a description list of my current studies and self-taught skills.
- **Contact** – my address details and a contact form (name, email, message) so visitors can reach me.
- **Aside** – a small "Current Focus" note.
- **Footer** – copyright and a "Back to Top" link.

The site uses well over 25 different HTML elements and more than 15 different HTML attributes, meeting the assignment's technical requirements.

## Question 2: HTML Elements

**1. Which 5 elements did I find most challenging to implement and why?**

- `<table>` – Getting the `<thead>`/`<tbody>` split and aligning columns (Project Name, Description, Tech Used, Status) correctly took some trial and error.
- `<form>` – Understanding the difference between `<label for="...">` and the matching input `id`, and choosing correct `type` values for each field (text, email, submit, reset), was tricky at first.
- `<dl>` (description list) – Pairing `<dt>` and `<dd>` correctly for my Education section wasn't something I had used before.
- `<details>`/`<summary>` – Getting the collapsible "tools I use" box to behave as expected took some testing.
- `<abbr>` – Remembering to use the `title` attribute so the abbreviation ("HTML") shows an explanation on hover.

**2. How did I use semantic elements to structure my content?**

I used `<header>` for my name/tagline/navigation, `<nav>` for the menu links, `<main>` to wrap the primary page content, `<section>` for each major topic (About, Skills, Projects, Education, Contact), `<article>` for my self-contained "About Me" bio, `<aside>` for the secondary "Current Focus" note, and `<footer>` for the copyright/back-to-top area. This gives the page a logical, screen-reader-friendly structure instead of relying only on generic `<div>`s.

**3. Which element was most useful for organizing my layout and why?**

`<section>` was the most useful element. Splitting the page into `id`-tagged sections (`about`, `skills`, `projects`, `education`, `contact`) let me build clean, independent blocks of content and also gave me anchor targets for my navigation links (`#about`, `#skills`, etc.), so visitors can jump straight to the part of the page they want.

## Question 3: HTML Attributes

**1. Which 3 attributes were essential for making my website functional?**

- `href` – makes the navigation links and the "Back to Top" link actually take visitors to the right section or page.
- `id` – gives each section a unique anchor so the in-page navigation links can jump to the correct part of the page, and lets `<label for="">` connect to the right form field.
- `type` – defines the correct behaviour for form inputs (`text`, `email`, `submit`, `reset`) and for lists (`type="square"` on my skills list).

**2. How did I use the `class` and `id` attributes differently?**

In this version of the site I relied mainly on `id` (e.g. `id="about"`, `id="skills"`, `id="projects"`, `id="name"`, `id="email"`) to mark unique elements that needed to be targeted individually — either as navigation anchors or as form field identifiers linked to their `<label>`. I did not need `class` here since every styled/targeted element only occurs once on the page, but in a future version with CSS I would use `class` to apply a shared style to repeated elements (e.g. all project rows) while keeping `id` reserved for one-of-a-kind elements.

**3. Which attribute helped improve user experience the most and why?**

The `placeholder` attribute on my form inputs (name, email, message) improved user experience the most, because it shows example text inside empty fields, guiding visitors on what to type without needing extra instructions. Close behind it, `required` ensures visitors can't submit the contact form without filling in their name and email, preventing incomplete submissions.

## Question 4: Development Process

**1. How did I plan my website structure before coding?**

I first listed the sections I wanted a portfolio to have — About, Skills, Projects, Education, and Contact — and decided on a single-page layout with a navigation bar linking to each section by anchor. I then sketched out, section by section, which HTML elements would best represent that content (a table for projects, a list for skills, a form for contact, etc.) before writing any code.

**2. What was my approach to testing and debugging my HTML?**

I built the page section by section and reloaded it in the browser (Live Server) after each change to check that the layout and links worked as expected. I checked that each navigation link scrolled to the correct section `id`, that the table rendered with visible borders and columns, and that the form fields lined up with their labels.

**3. What challenges did I face and how did I overcome them?**

My biggest challenges were remembering the correct nesting for less common elements like `<dl>`/`<dt>`/`<dd>` and `<thead>`/`<tbody>`, and making sure every `<label for="">` matched its input's `id` exactly. I overcame these by testing the page in the browser after every section and comparing my markup against HTML reference documentation to confirm correct syntax and attribute usage.

## Question 5: Git & GitHub Implementation

**1. What Git commands did I use during development?**

I used `git init` to start the repository, `git add .` to stage my files, `git commit -m "message"` to save progress at each stage, `git status` to check what had changed, and `git push` to upload my commits to GitHub.

**2. How many commits did I make and what was my commit message strategy?**

[Fill in with your actual commit count, e.g. "I made X commits."] My strategy was to commit after completing each major section of the website (e.g. "Add header and navigation", "Add skills section", "Add projects table", "Add contact form"), so each commit represents one clear, reviewable step in the site's development rather than one large, unclear commit.

**3. Why is version control important for web development projects?**

Version control lets me track exactly how my website changed over time, revert to an earlier version if something breaks, and keep a clear history of my progress. It also makes it possible to collaborate with others (such as adding an instructor as a collaborator) and back up my work outside of my local machine.

## Question 6: Code Quality & Best Practices

**1. How did I ensure my HTML was valid and error-free?**

I checked my markup for correctly closed tags, matching opening/closing pairs, and properly nested elements (e.g. `<tr>` inside `<tbody>`, `<dd>` following `<dt>`), and I tested the page in the browser to confirm it rendered and behaved as intended. I would also run the file through the W3C HTML validator to catch any remaining syntax issues.

**2. What best practices did I follow for writing clean, readable code?**

I used semantic elements instead of generic `<div>`s wherever possible, gave meaningful `id` names that match their section's purpose (`about`, `skills`, `projects`), kept related content grouped inside its own `<section>`/`<article>`, added `alt` text to my image for accessibility, and used consistent indentation to keep the structure easy to read.

**3. How would you improve your website if you had more time?**

I would add external CSS to style the page properly (my current version still has some legacy presentational attributes like `bgcolor` and `text` that should be replaced with CSS), fix small typos in the markup (e.g. the malformed `abbr title` attribute and the empty mailto link in the Contact section), make the navigation menu links more concise, and eventually add JavaScript for form validation and interactive effects like the cyber-terminal UI mentioned in my projects table.

## Technical Requirements Checklist

- [x] 25+ different HTML elements used (html, head, meta, title, body, header, h1, p, em, hr, nav, a, main, section, h2, article, img, strong, mark, abbr, blockquote, h3, ul, li, ol, details, summary, table, caption, thead, tr, th, tbody, td, br, dl, dt, dd, address, form, label, input, textarea, aside, footer)
- [x] 15+ different HTML attributes used (lang, charset, name, content, id, href, title, src, alt, width, height, border, cite, type, start, action, method, for, placeholder, required, size, rows, cols, value, target)
- [x] Semantic HTML structure implemented
- [x] Website works in web browser
- [ ] GitHub repository with all code
- [ ] README.md file with documentation (this file)
- [ ] Instructor added as collaborator (username: instructor-webdev / Billypeterlennards)
- [ ] Instructor followed on GitHub
- [ ] Google Classroom submission completed
