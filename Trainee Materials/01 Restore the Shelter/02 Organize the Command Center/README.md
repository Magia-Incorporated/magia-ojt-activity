# 02 — Organize the Command Center

**Chapter:** Restore the Shelter

**Work:** self-guided, individual, and AI-free. Use fictional exercise data only.

**Start here:** Complete Activity 01 first. Continue the same project.

## Mission briefing

Operators can read the recovered page, but the crowded layout slows them down. Make the terminal readable on a narrow screen and usable with a keyboard.

## Learn: selectors and the box model

```css
.radio-panel {
  padding: 1rem;
  border: 1px solid #888;
  margin-block: 1rem;
}
```

Padding creates space inside a border; margin separates elements outside it. A class selects a reusable group of elements. Try changing each spacing value independently and inspect the result with browser developer tools.

## Implementation steps

1. Create `web/styles.css`. Inside the `<head>` of `web/index.html`, add `<link rel="stylesheet" href="styles.css">`. This relative URL points from the HTML file to its neighboring stylesheet.
2. Apply a readable font, line height, page background, and foreground color.
3. Give the main content a maximum width and comfortable side padding. Use relative units.
4. Make the status/supply sections a simple Grid or Flexbox layout that collapses to one column on narrow screens.
5. Keep links recognizable and keyboard focus visible. A status must have words as well as any color or icon.
6. Use the browser’s computed styles and box-model inspector to explain one layout decision.

## Independent task

Add a visual status panel reading **Remote relay offline**. It must remain understandable without color. At about 320 CSS pixels wide, the page must remain readable without horizontal page scrolling. Avoid a fixed width larger than the viewport.

## Check and expected output

- Check a narrow viewport and a desktop viewport; record what you inspected in `docs/activity-02.md`.
- Tab through every link and confirm a visible focus indicator.
- Zoom the browser to 200% and check that content remains reachable.
- Temporarily remove the stylesheet; the document should retain a useful reading order.

There is no single required color scheme. Check that you can explain contrast, spacing, and the rule responsible for the responsive layout.

## Git checkpoint

Use your existing Git workflow to inspect the changed files, stage only the intended source/notes, review the staged diff, commit with a useful message, and push to personal `main`.

Record the commit or PR link and your checks in `docs/activity-02.md` (create the docs folder if needed). Do not upload personal details or private answer keys. A local commit alone is not on GitHub.

References: [CSS box model](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Box_model), [responsive design](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design).

Return to the [chapter briefing](../README.md).
