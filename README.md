# Scale Propagation Network — OMEGA Lab project page

Project page for **Scale Propagation Network for Generalizable Depth Completion**, in the OMEGA
Lab style.

- Paper: <https://arxiv.org/abs/2410.18408> (IEEE TPAMI: <https://doi.org/10.1109/TPAMI.2024.3513440>)
- Code: <https://github.com/Wang-xjtu/SPNet>
- Page: <https://omega-hkustgz.github.io/projects/scale-propagation-network/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/`; there is no build step. Rules for agents are in
[`AGENTS.md`](AGENTS.md).

```sh
node tools/check.mjs     # what CI runs
node tools/serve.mjs     # look at it locally
```

Every pull request gets a preview link, posted on the pull request. A push to `main` asks the
lab site to republish.

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2410.18408v1 (24 Oct 2024). The text paraphrases the abstract and Sections III–VI; it adds no claims. The paper lists affiliations in IEEE footnotes without superscripts; the superscripts on the page follow those footnotes. |
| Venue, DOI, BibTeX | IEEE TPAMI 47(3), 1908–1922, 2025, DOI 10.1109/TPAMI.2024.3513440, as recorded in the lab site's `publications.json` and in the code repository's README. |
| `teaser.webp`, `sp-norm.webp`, `network.webp`, `qualitative.webp`, `sparsity.webp`, `light-conditions.webp` | Figs. 1, 4, 6, 8, 10 and 11 of the paper, from the raster figure files in the arXiv source (resized to at most 2400 px wide with `magick`, then `cwebp -q 90`). `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. The cover image on the first author's homepage (`SPNet.jpg`, fetched 2026-11-10) is the same figure at lower resolution and was not used. |
| Random-pixel and LiDAR/holes tables, headline numbers | Tables II and III of the paper, copied from the LaTeX source. |
| Retrained-baseline, speed, robustness and ablation numbers in the text | Tables IV–XI and Sections V-B to V-D of the paper. |
| Code button and the list of released materials | The authors' repository <https://github.com/Wang-xjtu/SPNet> (README at commit `b836bd0`, 1 Apr 2025): training and test code, four pretrained models, a test dataset and two example training sets. |

Not on the page because no public material exists: demo videos or any footage of the model
running on a sensor or robot (the paper evaluates on benchmark datasets only, so the page has no
Demos section), and the ablation tables (Tables VII–XI, left to the paper).
