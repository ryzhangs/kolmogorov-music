# kolmogorov-music
Kolmogorov Complexity and Music Website

## Files

- `index.html` — title page and outline; each outline heading links to its section page.
- `01-introduction.html` … `08-classifying.html`, `references.html` — one page per section.
- `style.css` — all styling, shared by every page.
- `math.js` — MathJax settings (`$…$` inline, `$$…$$` display, numbered `\begin{equation}`).

## Writing a section

Open the section's page and write between the `WRITE THIS SECTION BELOW` and `END OF SECTION` comments.
Replace each `<p class="todo">To write.</p>` placeholder with your text. Subsections are `<h2>`; sub-subsections are `<h3>`.

Building blocks you can paste in:

```html
<p>Plain paragraph with inline math $K(x) \le |x| + c$.</p>

$$K_U(x) = \min\{|p| : U(p) = x\}$$

<div class="box definition">
  <p class="box-title">Definition 1.1 <span class="name">(Kolmogorov complexity)</span></p>
  <p>…</p>
</div>

<div class="box theorem">
  <p class="box-title">Theorem 2.1 <span class="name">(Invariance)</span></p>
  <p>…</p>
</div>

<div class="proof">
  <p>…</p>          <!-- "Proof." and the ∎ are added automatically -->
</div>

<div class="box example">
  <p class="box-title">Example</p>
  <p>…</p>
</div>

<pre>python or pseudocode</pre>

<figure>
  <img src="media/tree.png" alt="…">
  <figcaption>Caption.</figcaption>
</figure>
```

Preview locally with `python3 -m http.server` in this folder, then open http://localhost:8000.
