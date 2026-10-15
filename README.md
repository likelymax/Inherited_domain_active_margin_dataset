# Lower Crustal Density in Active Continental Margins

This repository contains the lower-crustal density (`rho_lc`) datasets used in the study:

**Lower Crustal Density Records Inherited Structure in Active Continental Margins**

The datasets provide lower-crustal density estimates for three active continental margins: **Chile, Cascadia, and Alaska**. Lower-crustal density was estimated from receiver-function amplitudes using the method described by Wang et al. (2025).

The study investigates how lower-crustal density varies with inherited tectonic structure and active-margin processes.

## Repository Contents

The repository contains four text files:

- `Chile_lower_crustal_density.txt`
- `Cascadia_lower_crustal_density.txt`
- `Alaska_CVM_lower_crustal_density.txt`
- `Alaska_AK112_lower_crustal_density.txt`

Each file contains lower-crustal density estimates at Moho piercing-point locations together with the associated propagated uncertainty.

## Data Format

Each dataset contains the following columns:

| Column | Description | Unit |
|---|---|---|
| `longitude` | Longitude of the Moho piercing point | degrees |
| `latitude` | Latitude of the Moho piercing point | degrees |
| `density` | Estimated lower-crustal density (`rho_lc`) | g/cm³ |
| `uncertainty` | Propagated uncertainty of the density estimate | g/cm³ |
| `percentage` | Relative uncertainty | % |

Only density estimates passing the quality-control criteria used in the study are included.

## Study Regions and Velocity Models

### Chile

**File:** `Chile_lower_crustal_density.txt`

**Study region:**  
77°W–63°W, 34°S–12°S

The study area covers the western South American active margin from the coastal forearc through the Andean volcanic arc and into the inland/backarc region.

**Velocity model:**  
SENAM_FWT2021 (FWT) South America shear-wave velocity model (Li and Gao, 2021).

The FWT model provides the lower-crustal and upper-mantle shear-wave velocities used in the density calculation. Because the model provides shear-wave velocity but not compressional-wave velocity, `Vp` was estimated using a constant `Vp/Vs = 1.8`.

---

### Cascadia

**File:** `Cascadia_lower_crustal_density.txt`

**Study region:**  
130°W–116°W, 40°N–50°N

The study area extends across the Cascadia active continental margin, including the forearc, Cascade volcanic arc, and inland/backarc regions.

**Velocity model:**  
Shen and Ritzwoller (2016; SR) 3-D shear-wave velocity model.

The model is based on joint inversion of surface-wave dispersion, Rayleigh-wave H/V ratios, and receiver functions and provides lower-crustal and uppermost-mantle velocity structure across the Cascadia region.

---

### Alaska — CVM

**File:** `Alaska_CVM_lower_crustal_density.txt`

**Study region:**  
170°W–140°W, 55°N–65°N

The study area covers southern and central Alaska across the forearc, volcanic-arc, accreted-terrane, and continental-interior regions.

**Velocity model:**  
Alaska Community Velocity Model, `Alaska_CVM_AKAN2020` (CVM; Nayak et al., 2020).

CVM provides laterally varying crustal and upper-mantle velocity structure across Alaska. This model is used as the **primary Alaska velocity model** in the associated study because it provides broader spatial coverage.

---

### Alaska — AK112

**File:** `Alaska_AK112_lower_crustal_density.txt`

**Study region:**  
170°W–140°W, 55°N–65°N

This dataset covers the same Alaska study region as the CVM dataset.

**Velocity model:**  
AK112 regional velocity model (Rodgers, 2025).

AK112 is based on 3-D full-waveform inversion tomography and provides an independent regional velocity model for Alaska. The AK112-derived density estimates are included as an independent comparison used to evaluate the sensitivity of the Alaska results to velocity-model choice.

The same lower-crustal density calculation and quality-control procedure was applied to the CVM and AK112 datasets.

## Method Summary

Lower-crustal density was calculated using receiver-function amplitude constraints following Wang et al. (2025). The method uses the transmission coefficient of the Moho P-to-S conversion, constrained by the amplitude ratio between the Moho-converted `Ps` phase and the direct `P` phase.

The calculation uses:

- lower-crustal `Vp` and `Vs`
- upper-mantle `Vp` and `Vs`
- seismic ray parameter
- upper-mantle density
- receiver-function `Ps/P` amplitude ratio

The same processing and quality-control framework was applied across Chile, Cascadia, and Alaska to permit direct regional comparisons.

## Geographic Coordinates

Coordinates in the files represent the geographic locations associated with the lower-crustal density estimates at the **Moho piercing points**, rather than simply the locations of the seismic stations.

Longitude and latitude are given in decimal degrees:

- negative longitude = west
- negative latitude = south

## Associated Study

These datasets accompany the manuscript:

**Wang, Y. — Lower Crustal Density Records Inherited Structure in Active Continental Margins**

The study compares lower-crustal density across Chile, Cascadia, and Alaska to evaluate the relative roles of inherited tectonic structure and active-margin magmatic and thermal modification.

## Related Method

The lower-crustal density calculation follows:

Wang et al. (2025), *Lower Crustal Density: Method and Uncertainty Quantification*, Seismological Research Letters.

DOI: 10.1785/0220250233

## Citation

If you use these datasets, please cite the associated manuscript and the lower-crustal density methodology paper.

A complete citation for the associated manuscript will be added after publication.

## Contact

**Yitan Wang**  
Independent Researcher  
Bellevue, Washington, USA  
Email: ytwang.geophysics@gmail.com
