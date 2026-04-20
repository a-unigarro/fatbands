# Fatbands Analysis Tools

Python tools for extracting and plotting fatband projections from electronic structure calculations. 

Developed for **ABINIT v.9.10.3**, this tool parses NetCDF output to visualize the contribution of atomic orbitals to the electronic band structure.

## Features
- **Core Data Extraction:** High-performance parsing of NetCDF files using `xarray`.
- **L-resolved plots:** Visualize orbital angular momentum contributions ($s, p, d, f$). 
- **LM-resolved plots:** Visualize magnetic quantum number projections (e.g., $d_{xy}, d_{z^2}$).
- **Spin Polarization:** Automatic handling of spin-up and spin-down channels with distinct markers ("^" and "v").

## ABINIT Requirements
To generate the compatible input files (`FATBANDS.nc`), your ABINIT input file (`.abi`) must include the following flags:

* **For L-resolved plots:** `prtdos = 3`
* **For LM-resolved plots:** `prtdos = 3` and `prtdosm != 0`

---

## Install Dependencies 
pip install -r requirements.txt


## Usage
Check example.py file
