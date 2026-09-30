# Data

All files in this folder are from the publicly released AlSi10Mg PBF-LB dataset by:

> Luo, Q., Huang, N., Fu, T., Wang, J., Bartles, D.L., Simpson, T.W., & Beese, A.M. (2023). New insight into the multivariate relationships among process, structure, and properties in laser powder bed fusion AlSi10Mg. *Additive Manufacturing*, 77, 103804. https://doi.org/10.1016/j.addma.2023.103804

Original dataset, released under **CC BY 4.0**:
**https://zenodo.org/records/10008435**

Re-hosted here, with attribution, for the purposes of this ontology-engineering project. All credit for data collection, experimental design, and the underlying materials-science analysis belongs to the original authors. This project does not modify the measured values; it only reorganizes and represents them for the knowledge graph.

## Files

**`AlSi10Mg_PSP_feature_table.xlsx`**
The master summary table. One row per processing parameter set (60 total), with every summary feature side by side: processing inputs (laser power, scan speed, hatch spacing, layer thickness), the derived energy-density descriptors (VED, MVED, PV), and every structural and mechanical property, each already averaged with its standard deviation.

**`_FR__Archimedes_porosity_table.xlsx`**
Raw dry-weight and submerged-weight readings behind the Archimedes porosity values — three weighings per sample, before averaging.

**`_FR__Mechanical_property_table.xlsx`**
UTS, yield strength, and elongation, broken out per physical replicate specimen (three per processing parameter set), before averaging into the master table.

**`_FR__Sample_geometry_table.xlsx`**
Caliper measurements (width, thickness) of each replicate specimen, used to normalize the tensile test results.

**`_FR__Surface_roughness_table.xlsx`**
Individual surface roughness readings per sample, before averaging into the master table's average and RMS values.

**`_FR__Vickers_microhardness_table.xlsx`**
Ten individual hardness indent readings per sample, before averaging into the master table's single hardness value.

**`Defect_pore_morphology.zip`**
Per-sample CSV files listing every individual pore found by X-ray CT in that sample — size, shape, and sphericity — before aggregation into one sample-level porosity percentage.

**`Grain-cell_morphology.zip`**
Raw per-cell area measurements from SEM imaging, before aggregation into the master table's cell-size averages.

**`Stress-strain_curves.zip`**
Full stress-strain curve for each of the three replicate specimens per sample, before reduction to the master table's UTS/yield/elongation/modulus values.
