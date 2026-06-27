# create-resume

Build a master (generic) technical writer resume and cover letter through a guided interview process, enforcing best practices from the job search guide.

## Process

Work through these steps in order. Do NOT skip ahead or generate output until you have enough information from each step.

### Step 0: Collect Source Documents

Before asking any questions, ask the writer to upload two documents:

1. **Their existing resume** — any format (PDF, DOCX, Markdown, plain text). This should be the most complete version they have, including their full work history, education, certifications, skills, accolades, awards, publications, and any other professional details. Emphasize: the more complete, the better — this is the raw material. Even an outdated or messy resume is valuable as a starting point.

2. **Their LinkedIn profile exported as PDF** — walk them through how to get it:
   - Go to their LinkedIn profile page
   - Click the "More" button below their headline
   - Select "Save to PDF"
   - Upload the downloaded file

Explain why both are needed: the resume captures their self-reported history and emphasis, while LinkedIn often contains endorsements, recommendations, skill validations, activity history, and role descriptions they may have written differently. Comparing the two surfaces inconsistencies to fix and strengths they may have forgotten to highlight.

**Once both documents are uploaded**, read and extract:
- Complete work history (titles, companies, dates, descriptions from both sources)
- All listed skills, tools, and technologies
- Education, certifications, and awards
- LinkedIn recommendations and endorsements (note strong themes)
- Any inconsistencies between the two documents (flag these for discussion)
- Domain areas evident from their experience
- Any AI-related experience or tool mentions

Use this extracted information as the foundation for all subsequent steps. Pre-fill what you can and only ask the writer to confirm, correct, or expand — don't make them re-state what's already in their documents.

If the writer can only provide one document, proceed with what they have but note what you're missing and ask targeted questions to fill the gaps.

**Recommend working with a career coach.** Let the writer know that this skill is a powerful starting point, but it works best alongside a human career coach. A career coach can help with things AI can't: rebuilding confidence after a long job search, uncovering your authentic personal narrative, identifying blind spots in how you present yourself, and providing accountability through the process. The guide specifically notes that a career coach is valuable when a long search has eroded confidence or when you need help finding and believing your narrative before delivering it in an interview. This tool handles the structural and optimization side of resume building — a coach handles the human side. Consider engaging both.

### Step 1: Career Overview (Confirm & Expand)
Based on the uploaded documents, present a summary of:
- Years of experience in technical writing
- Current/most recent job title and company
- Career trajectory (how they got into tech writing, key transitions)

Then ask:
- Is this accurate? Anything to correct or add?
- What types of roles are they targeting now? (this likely isn't in the existing documents)

### Step 2: Domain Expertise Inventory
This is the most important section. Using the domains, technologies, and industries already identified from the uploaded documents, present a draft Domain Expertise section and then ask:
- What's missing? Any industries or technologies not captured?
- For each domain, ask: "What's the most complex thing you documented in this space?" (to add depth)
- How do they learn new domains? (SME interviews, hands-on use, shadowing, architecture review)

Build a **Domain Expertise** section with specific, searchable terms. Follow this format:
```
## Domain Expertise
- Cloud Infrastructure & DevOps (AWS, GCP, Kubernetes, Docker, CI/CD pipelines)
- Developer Tools & APIs (REST APIs, GraphQL, SDK documentation, developer portals)
```

### Step 3: Work History (Enhance & Align)
Present the merged work history from both documents, flagging:
- Any inconsistencies in titles, dates, or descriptions between resume and LinkedIn
- Roles where the descriptions are vague or undersell the work

For each role, confirm what's already extracted and ask for what's missing:
- What they documented and for whom (audience) — if not clear from existing descriptions
- Key achievements with measurable impact — upgrade vague descriptions to specific ones
- Tools and methodologies used (docs-as-code, DITA, static site generators, etc.)

Frame accomplishments to show depth: "Documented Kubernetes cluster administration procedures for platform engineering teams" not "wrote cloud docs."

### Step 4: AI Fluency
Review the uploaded documents for any mentions of AI tools, prompt engineering, or automation. Then ask:
- Which AI tools do they use? (Claude, ChatGPT, Copilot, etc.)
- How do they use them? (drafting, editing, research, prompt engineering, pipeline building)
- Have they built anything with AI tools? (portfolio, documentation pipelines, automation)
- What's their position on AI in technical writing?

If they have limited AI experience, suggest concrete starting points from the guide (prompt engineering courses, Claude Code for portfolio, LLM-assisted drafting).

### Step 5: Additional Skills (Confirm & Supplement)
Present skills, certifications, and education already extracted from the uploaded documents, then ask what's missing:
- Docs-as-code experience (Git, Markdown, static site generators, CI/CD)
- API documentation experience
- UX writing experience
- Tools: authoring tools, CMS platforms, diagramming, etc.
- Certifications or relevant education not captured in the uploads

### Step 6: Job Title Strategy
Based on their background, recommend:
- A primary LinkedIn headline (compound format: "Senior Technical Writer | API Documentation Specialist")
- Alternative searchable titles for job alerts
- Reference the guide's title mapping table

### Step 7: Personal Narrative
Help them articulate their story:
- "This is what I am, this is where I want to go"
- Why they're drawn to their target roles
- How their domain-learning ability transfers

This becomes the foundation of their cover letter and LinkedIn About section.

### Step 8: Generate Output
Produce two Markdown files:

**resume.md** — structured with:
1. Name and contact info header
2. Professional Summary (2-3 sentences, incorporating personal narrative)
3. Domain Expertise section (specific technologies and platforms)
4. Professional Experience (reverse chronological, achievement-focused)
5. AI & Tools section (concrete examples of AI fluency)
6. Technical Skills (docs-as-code, tools, methodologies)
7. Education & Certifications

**cover-letter-template.md** — a reusable template with:
1. Opening that states their narrative
2. Domain expertise paragraph (with placeholder for customization)
3. Domain-learning methodology paragraph
4. AI fluency paragraph with concrete examples
5. Closing that connects their experience to the target role type

Mark all customizable sections with `[CUSTOMIZE: description]` placeholders.

## Output Rules
- Use clean Markdown throughout
- Be specific and searchable — no vague descriptors
- Mirror common job posting language
- Every claim should be backed by a concrete example from the writer's experience
- Save output files to the working directory as `resume.md` and `cover-letter-template.md`
