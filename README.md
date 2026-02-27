# Perlin Noise Exploration

Exploring Perlin noise fundamentals with Python and Jupyter notebooks.

This notebook walks through the mathematical foundations of Perlin noise, starting from linear interpolation and building up to gradient noise with smoothstep functions.

## View Online

[View the rendered notebook](https://perlin-noise-exploration.pages.dev)

## Topics Covered

- Linear interpolation (LERP) between lines
- Gradient noise fundamentals
- Smoothstep/fade function: `6t^5 - 15t^4 + 10t^3`
- 1D Perlin noise implementation
- Visualization with matplotlib

## Running the Notebook

1. Create a virtual environment and install dependencies:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

2. Launch the notebook:

```bash
jupyter notebook Perlin_noise.ipynb
```

## Rendering HTML

The notebook is rendered to a static HTML page using [Quarto](https://quarto.org/). The theme and output format are configured in `_quarto.yml`.

To render locally:

```bash
quarto render Perlin_noise.ipynb --to html --output-dir docs
```

This produces `docs/Perlin_noise.html` along with image assets in `docs/Perlin_noise_files/`. Rename the HTML to `index.html` for deployment:

```bash
mv docs/Perlin_noise.html docs/index.html
```

## Deployment

The site is automatically deployed to [Cloudflare Pages](https://pages.cloudflare.com/) via a GitHub Actions workflow (`.github/workflows/deploy.yml`). Every push to `master` triggers the workflow, which uses the Cloudflare Wrangler action to deploy the contents of `docs/` to the project `perlin-noise-exploration`.

The workflow requires two GitHub repository secrets:

- `CLOUDFLARE_API_TOKEN`
- `CLOUDFLARE_ACCOUNT_ID`
