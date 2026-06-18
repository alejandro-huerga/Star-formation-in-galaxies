# Galactic Chemical Evolution Model of the Milky Way

Numerical model of galactic chemical evolution implemented in Python,
developed as an undergraduate research thesis (TFG) at the Autonomous
University of Madrid (UAM).

## Description

The model solves the coupled evolution of gas mass, stellar mass, and
turbulent energy across the Milky Way disk using a radial ring
decomposition approach. Each annular ring evolves independently,
allowing radial profile predictions to be compared against observations.

Physical processes implemented:
- **Gas accretion**: exponential infall with radially varying timescale
- **Star formation**: Schmidt-type law with free-fall time regulation
- **Supernova feedback**: turbulent energy injection and radiative
  cooling (Sedov-Taylor cooling timescale)
- **Vertical disk structure**: scale height z₀ and central density ρ₀
- **Inside-out formation**: linearly increasing infall timescale with radius
- **Disk stability**: Toomre-Q diagnostics and gas depletion timescales

Model predictions are compared against observed Milky Way radial profiles
(stellar surface density, gas surface density, SFR) from
Mollá et al. (2015), MNRAS, 451, 3693.

## Requirements

Python 3.10+ recommended.

pip install -r requirements.txt

Dependencies: numpy, scipy, matplotlib, astropy, ipykernel

## Usage

Open and run Analysis_star_formation_1.ipynb in Jupyter.
The notebook is organized in self-contained sections with markdown
headers. Each section can be run independently after the initial
setup cell.

## Output

The notebook generates publication-quality PDF figures including:
- Mass and velocity dispersion evolution (single ring)
- Toomre-Q stability and disk scale height evolution
- Radial profiles of stellar density, gas density, SFR,
  and gas depletion time compared with Mollá et al. (2015)
- Comparison between fast and constant infall scenarios
