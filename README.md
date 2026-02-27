# Perlin Noise Exploration

Exploring Perlin noise fundamentals with Python and Jupyter notebooks.

This notebook walks through the mathematical foundations of Perlin noise, starting from linear interpolation and building up to gradient noise with smoothstep functions.

## Setup

1. Create a virtual environment:

```bash
python3 -m venv myenv
source myenv/bin/activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Notebook

```bash
jupyter notebook Perlin_noise.ipynb
```

## Topics Covered

- Linear interpolation (LERP) between lines
- Gradient noise fundamentals
- Smoothstep/fade function: `6t^5 - 15t^4 + 10t^3`
- 1D Perlin noise implementation
- Visualization with matplotlib
