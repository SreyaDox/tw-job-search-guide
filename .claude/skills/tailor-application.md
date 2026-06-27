# tailor-application

Take an existing generic resume and a specific job posting, then produce a tailored resume and cover letter optimized for that role. Enforces ATS optimization and domain-alignment best practices from the job search guide.

## Inputs Required

Ask the writer for:
1. **Generic resume** — their master resume (Markdown preferred, or paste content). If they used `/create-resume`, reference that output.
2. **Job posting** — the full text of the target job posting (URL or pasted content). If a URL is provided, fetch it.

## Process

### Step 1: Analyze the Job Posting
Extract and present to the writer:
- **Required qualifications** (hard requirements vs. nice-to-haves)
- **Key terms and phrases** that must appear in the tailored resume (exact language from the posting)
- **Domain focus** — what industry/technology domain is this role in?
- **Audience** — who will this writer be writing for? (developers, end users, internal teams, etc.)
- **ATS keywords** — specific tools, technologies, methodologies, and job titles mentioned

### Step 2: Gap Analysis
Compare the generic resume against the posting:
- **Strong matches** — domains, skills, and experience that directly align
- **Partial matches** — adjacent experience that can be reframed
- **Gaps** — requirements the writer may not meet; suggest how to address (transferable skills, learning narrative, or honest acknowledgment)

Present this analysis and ask the writer to confirm or add context before proceeding.

### Step 3: Tailor the Resume

Apply these transformations:

**Language mirroring:**
- Replace generic terms with the posting's exact language. If the posting says "developer documentation," use "developer documentation" — not "API docs" or "technical guides"
- Match their terminology for tools and platforms exactly

**Domain reordering:**
- Restructure the Domain Expertise section to lead with the domain that matches this role
- Add specificity for the matching domain; keep other domains but lower their prominence

**Title alignment:**
- Adjust the professional title/headline to match or closely mirror the posted job title
- Use compound format if needed: "Technical Writer | [Posted Title Keywords]"

**Experience emphasis:**
- Reorder or expand bullet points that demonstrate relevant experience
- Add keywords from the posting into existing achievement descriptions (without fabricating)
- Highlight AI fluency if the posting mentions it (most do now)

**Professional summary:**
- Rewrite to directly address this specific role and company
- Lead with the most relevant domain expertise
- Include 2-3 key terms from the posting naturally

### Step 4: Write the Tailored Cover Letter

Structure:
1. **Opening** — name the specific role and company; state why you're drawn to it (connect to personal narrative)
2. **Domain match** — your most relevant domain expertise and how it applies to their specific products/challenges
3. **Domain-learning methodology** — how you acquire deep product knowledge (SME interviews, hands-on use, architecture review) — this signals you can ramp up in their environment
4. **AI fluency** — concrete examples of how you use AI tools in documentation work (only if relevant to the posting; it usually is)
5. **Closing** — connect your trajectory to their needs; express genuine interest

Rules for the cover letter:
- Use the posting's exact terminology throughout
- Be specific to this company and role — generic cover letters are obvious and ineffective
- Keep it under one page (roughly 350-450 words)
- Maintain second-person self-reference style that's direct and confident, not boastful

### Step 5: Keyword Verification
Before delivering, verify:
- [ ] All key terms from the job posting appear at least once in the resume
- [ ] Job title in resume header matches or mirrors the posted title
- [ ] Domain Expertise section leads with the relevant domain
- [ ] Professional summary addresses this specific role
- [ ] Cover letter names the company and role specifically
- [ ] No fabricated experience — all claims map to the writer's actual background
- [ ] Language mirrors the posting (not paraphrased into different terms)

Present the checklist results to the writer.

### Step 6: Generate Output

Save two files:
- `resume-[company-slug].md` — the tailored resume
- `cover-letter-[company-slug].md` — the tailored cover letter

Where `[company-slug]` is a lowercase, hyphenated version of the company name.

## Output Rules
- Clean Markdown format
- Every keyword from the posting should appear naturally in the resume or cover letter
- Never fabricate experience — reframe existing experience using the posting's language
- Flag any significant gaps honestly so the writer can decide how to address them
- If the role is a major domain shift, suggest framing from the guide's "Crossing into new industries" section
