Both render identically. But the semantic version tells Google, screen readers, and other machines what each region *is*. The `<nav>` tells Google "these are navigation links." The `<article>` tells a screen reader "this is a self-contained piece of content." The `<footer>` tells a scraper "this is page metadata."The landmark roles are a big deal in accessibility. A blind user with a screen reader can press a key to jump directly to `<main>`, skipping the nav. If you use `<div>` everywhere, that ability disappears.

---

## Part 4: Text-Level Semantic Tags The Inline Elements

These go *inside* paragraphs and headings. Each has specific meaning that affects accessibility, SEO, and styling.

```html
<p>
  The word <strong>danger</strong> carries high importance.
  The word <em>slowly</em> is being emphasized for tone.
  The abbreviation <abbr title="HyperText Markup Language">HTML</abbr> is explained on hover.
  This is a <mark>highlighted passage</mark> for reference.
  The price dropped from <del>₹500</del> to <ins>₹350</ins>.
  The formula is H<sub>2</sub>O and E=mc<sup>2</sup>.
  The error code was <code>404 Not Found</code>.
  Press <kbd>Ctrl</kbd> + <kbd>S</kbd> to save.
  The output was <samp>Hello, World!</samp>.
  The variable is defined as <var>x</var>.
  <q>To be or not to be</q> is a famous quote.
  <cite>Hamlet</cite> was written by Shakespeare.
  This is <small>fine print or legal text</small>.
  A word break opportunity: super<wbr>cali<wbr>fragilistic
  <time datetime="2025-01-15">January 15, 2025</time>
</p>
```