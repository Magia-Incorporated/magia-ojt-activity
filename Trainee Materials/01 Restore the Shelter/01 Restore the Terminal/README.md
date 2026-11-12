# 01 — Restore the Terminal

**Chapter:** Restore the Shelter

**Work:** self-guided, individual, and AI-free. Use fictional exercise data only.

**Start here:** Use the project setup below; Git/GitHub basics are assumed complete.

## Mission briefing

Power has returned to the shelter, but its information terminal is blank. Build the first Survival Nexus page so the resistance can read shelter status and priority supplies.

## Project setup

Use the existing local checkout of your personal public `Survival-Nexus` repository. If the project repository does not exist yet, follow the short repository requirement in the course root README. Git/GitHub onboarding is already complete; there is no new account lesson, questionnaire, or Git quiz.

Open the project folder in your plain-text editor. Confirm that you can save files with their actual extensions rather than `.html.txt`. Create a `web` folder and a file named `index.html` inside it. Keep the course handouts in a separate folder from your application. Disable AI chat, agents, autocomplete, and AI search answers.

## Learn with a small working example

HTML gives content structure. Elements have opening/closing tags; attributes add information. A heading labels content, a paragraph contains text, and a section groups related information.

Try this complete smaller page in a temporary file called `radio-example.html`, outside your project’s tracked source:

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Radio Check</title>
</head>
<body>
  <h1>Radio Check</h1>
  <a href="#radio-status">Jump to status</a>
  <section id="radio-status">
    <h2>Channel status</h2>
    <p>The emergency channel is available.</p>
  </section>
</body>
</html>
```

Open it in a browser. Change the paragraph and reload. Notice that the document title appears in the browser tab, while h1 appears on the page. The link’s `#radio-status` matches the target element’s id. Read the linked HTML reference if any part is unfamiliar.

## Build the shelter terminal

Create your own `web/index.html` with document declaration, English language, UTF-8, viewport metadata, a useful title, and these body elements:

- A header with one main heading: **Survival Nexus**.
- A main area containing a short fictional mission description.
- A **Shelter status** section with two status messages.
- A **Priority supplies** section listing Water, Food, Medication, and C-Virus Vaccine using an unordered list.
- A **Communications** section with two technical status messages.
- Internal navigation links to Priority supplies and Communications, using matching IDs.
- A footer stating that the page uses fictional training data.

No JavaScript, external images, or framework is needed in this mission. Create or update your project README with a project title, current progress, and the instruction to open `web/index.html` in a browser.

## Check the result

1. Open the actual project file, not the example. Confirm the browser title and main heading.
2. Click both internal links. Each must move to its matching section.
3. Read the page from top to bottom: mission, shelter, supplies, communications, footer.
4. Check the source for one h1 and logical h2 section headings. Check opening/closing tag pairs and unique IDs.
5. Change a status message, save, and reload. Confirm the new text appears.

## Troubleshooting

- Browser shows source text: check that the file ends in `.html`, not `.txt`.
- Nothing changes after saving: verify the full file you opened is the one edited; save, then reload.
- Internal link does nothing: compare its href after # with the exact target id, including spelling.
- Content appears inside another section unexpectedly: inspect missing or mismatched closing tags.

## Git checkpoint

Use your existing Git workflow to inspect the changed files, stage only the intended source/notes, review the staged diff, commit with a useful message, and push to personal `main`.

Record the commit or PR link and your checks in `docs/activity-01.md` (create the docs folder if needed). Do not upload personal details or private answer keys. A local commit alone is not on GitHub.

## Completion checklist

- [ ] The required behavior matches every listed acceptance case.
- [ ] I wrote down actual results, including rejected/empty/boundary cases where specified.
- [ ] I can explain the important logic in my own technical notes.
- [ ] I completed the Git checkpoint and verified the pushed source.
- [ ] I used no AI or human hints, and my project contains only fictional exercise data.

If a check fails, use the [independent working guide](../../01%20Restore%20the%20Shelter/Working%20Independently.md), correct it, and rerun the relevant checks. Advance after your own checklist passes; no sign-off or live demonstration is required.

Reference: [MDN basic HTML syntax](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Basic_HTML_syntax).

Return to the [chapter briefing](../README.md).
