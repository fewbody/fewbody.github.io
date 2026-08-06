# QFBD Research Group website

Source for [fewbody.com](https://fewbody.com), the website of the Quantum Few-Body Dynamics (QFBD)
group led by Jin Lei at the Department of Physics, Tongji University, Shanghai.

Built with Jekyll and served by GitHub Pages from the `gh-pages` branch. Large downloads (seminar
slides, teaching code archives) live on the separate `downloads-storage` branch and are linked by
raw URL, which keeps this branch small.

## Editing

| What you want to change | File |
|---|---|
| Landing page | `_pages/home.md` |
| Research statement | `_pages/research.md` |
| Code list | `_pages/codes.md` |
| Recruiting page | `_pages/opening.md` |
| Publications | `_pages/publications.md` |
| People | `_data/team_members.yml`, `_data/students.yml`, `_data/alumni_members.yml` |
| News items | `_data/news.yml` |
| Seminars, group meetings | `_pages/seminar.md`, `_pages/groupmeeting.md` |
| Navigation, footer | `_includes/header.html`, `_includes/footer.html` |
| Styling | `css/main.scss` |

## Bilingual content

The site ships English and Chinese in the same page and switches between them with the button in
the navigation bar. Any element with class `l-en` is shown in English mode and any element with
class `l-zh` in Chinese mode; the choice is stored in `localStorage` under `qfbd-lang` and applied
before first paint, so the page never flashes the wrong language. English is the default for a
first-time visitor.

To add bilingual text, write both versions as sibling elements:

```html
<p class="l-en">English sentence.</p>
<p class="l-zh">中文句子。</p>
```

Data files follow the same pattern with a `_zh` suffix: `headline` and `headline_zh` in
`_data/news.yml`, `info` and `info_zh` in the people files. If the `_zh` field is missing, the
English text is shown in both modes, so a partial translation degrades gracefully.

## Publication list

`_pages/publications.md` is generated from the INSPIRE-HEP author record `Lei.Jin.2`, so every
journal, volume, page and DOI comes from a fetched record rather than being typed by hand. A few
titles that INSPIRE stores with embedded MathML are patched from an explicit table in the generator
script. Regenerate when new papers appear rather than editing entries by hand.

## Local preview

```
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>. Ruby 3.x is required by the current gem set.

## Credits

The layout descends from the [Allan Lab](https://github.com/allanlab/allanlab) Jekyll template
(Leiden University), heavily rewritten. Content and research material are the property of the QFBD
group, Tongji University.
