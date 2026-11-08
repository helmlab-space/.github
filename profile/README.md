# Helmlab

Color-space, measurement and data tools.

Helmlab defines color spaces for generating colors (gradients, palettes, gamut mapping) and for measuring color differences, and publishes their reference code. It also maintains a benchmark for color spaces and a pool of color-perception datasets.

## Current definition: Helmlab 2026

Helmlab 2026 is defined by the outputs of `helmlab` 1.0.0 on npm and PyPI. `helmlab` 1.0.1 has identical outputs; only its JavaScript speed and documentation changed.

| Identifier | What it names |
| --- | --- |
| `helmgen` | GenSpace in Lab coordinates, for generating colors |
| `helmgenlch` | GenSpace in LCh coordinates (lightness, chroma, hue) |
| `helmlab-metric` | MetricSpace, for measuring color differences |
| ΔE `helmlab` | Color difference computed from `helmlab-metric` coordinates |

A specification and test vectors for Helmlab 2026 are planned for the `helmlab` repository.

## Repositories

| Repository | Contents |
| --- | --- |
| [`helmlab`](https://github.com/Grkmyldz148/helmlab) | Reference code: the `helmlab` package for npm and PyPI. Also the `postcss-helmlab` plugin, the paper source and the sources of the agent skills. |
| [`colorbench`](https://github.com/Grkmyldz148/colorbench) | ColorBench tests color spaces against human psychophysical data and on generation properties such as gamut, gradients and round trips. Its public board shows pre-v4 results; those figures are withdrawn. |
| [`color-perception-datasets`](https://github.com/Grkmyldz148/color-perception-datasets) | Color-perception datasets in shared schemas. Each dataset's license is shown on its catalog page. The bulk download leaves out datasets whose license is unspecified or limited to academic or non-commercial use. |
| [`color-skills`](https://github.com/helmlab-space/color-skills) | Agent skills for color tasks, mirrored from the [`skills` folder](https://github.com/Grkmyldz148/helmlab/tree/main/skills) of `helmlab`. Install: `npx skills add helmlab-space/color-skills` |
| [`helmlab-experimental`](https://github.com/helmlab-space/helmlab-experimental) | Research experiments, optimization checkpoints and analysis scripts from GenSpace development. The win counts in its README are pre-v4 ColorBench figures. |

`helmlab`, `colorbench` and `color-perception-datasets` are under the maintainer's account, Grkmyldz148.

## Performance figures

Figures will be published on one evidence page, generated from one file. Each figure there will name its dataset, its size (n), and whether that data was used to fit, tune or design the model. The current version of the paper (arXiv v3) predates this rule. Figures from ColorBench before v4 and figures shown on the previous helmlab.space site are withdrawn.

## Links

- Packages: [`helmlab` on npm](https://www.npmjs.com/package/helmlab), [`helmlab` on PyPI](https://pypi.org/project/helmlab/), [`postcss-helmlab` on npm](https://www.npmjs.com/package/postcss-helmlab)
- Documentation: [`API.md`](https://github.com/Grkmyldz148/helmlab/blob/main/API.md) and [`CHANGELOG.md`](https://github.com/Grkmyldz148/helmlab/blob/main/CHANGELOG.md) in the `helmlab` repository
- Website: helmlab.space is offline; it is planned as the documentation site.
- Paper: [arXiv 2602.23010](https://arxiv.org/abs/2602.23010). Its description of the neutral-correction step differs from the released code; see [helmlab#4](https://github.com/Grkmyldz148/helmlab/issues/4).
- Dataset catalog: [grkmyldz148.github.io/color-perception-datasets](https://grkmyldz148.github.io/color-perception-datasets/)
- Questions and bug reports: open an issue in the relevant repository. Dataset takedown requests: [color-perception-datasets issues](https://github.com/Grkmyldz148/color-perception-datasets/issues).

Maintainer: [Görkem Yıldız](https://github.com/Grkmyldz148), author of the Helmlab spaces and of ColorBench.
