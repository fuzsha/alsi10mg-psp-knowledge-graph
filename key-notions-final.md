# Key Notions

* Sample
    * Rationale: One printed sample, with its own printing settings. Every number belongs to one sample.
    * Connected Pattern: Aggregation (member of a group), Quantity, Provenance, SOSA Observation (the thing observed), Explicit Typing
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx
    * Competency Questions: CQ1, CQ2, CQ3, CQ6, CQ7, CQ8, CQ9, CQ10, CQ11, CQ12, CQ16, CQ17
* Group
    * Rationale: A set of samples with the same hatch spacing: small (samples 1 to 32) or large (33 to 60). Samples are compared inside their own group.
    * Connected Pattern: Aggregation
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx
    * Competency Questions: CQ1, CQ2, CQ16
* Reported Value
    * Rationale: One final number for one sample, such as hardness, porosity or VED.
    * Connected Pattern: Quantity, SOSA Observation (the result), Data Transformation (the output), Provenance, Aggregation
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx
    * Competency Questions: CQ1, CQ2, CQ3, CQ4, CQ5, CQ6, CQ7, CQ8, CQ10, CQ12, CQ13, CQ14, CQ15, CQ18
* Process Parameter
    * Rationale: A printing setting chosen by the researchers: laser power, scan speed, hatch spacing, layer thickness.
    * Connected Pattern: Quantity, Data Transformation (a setting a calculation uses)
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx (printing settings columns)
    * Competency Questions: CQ3, CQ4, CQ7, CQ10, CQ11, CQ15, CQ17
* Label
    * Rationale: The kind of number (hardness, porosity, laser power). It also tells whether the number is a setting, observed, or calculated.
    * Connected Pattern: Quantity, Data Transformation, SOSA Observation (the property observed), Provenance, Aggregation
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx (column headers)
    * Competency Questions: CQ1, CQ2, CQ3, CQ4, CQ6, CQ7, CQ8, CQ10, CQ12, CQ14, CQ17, CQ18
* Raw Data
    * Rationale: One single reading behind a final number: one hardness dent, one pore, one weighing.
    * Connected Pattern: Aggregation (readings kept together), Provenance, Data Transformation (a setting a calculation uses)
    * Source Dataset(s): [FR] Vickers microhardness, Mechanical property, Surface roughness and Archimedes porosity tables; Defect pore morphology.zip; Grain-cell morphology.zip
    * Competency Questions: CQ2, CQ5, CQ8, CQ13, CQ15
* Calculation
    * Rationale: The step that makes a final number from readings or settings (an average, a formula).
    * Connected Pattern: Data Transformation
    * Source Dataset(s): matched from the master table to the raw files, plus the paper's methods section
    * Competency Questions: CQ4, CQ5, CQ10, CQ15
* Algorithm
    * Rationale: The formula or method a calculation follows, such as VED = P / (v x h x t) or the average of 10 readings.
    * Connected Pattern: Data Transformation
    * Source Dataset(s): worked out by us from the master table and raw files
    * Competency Questions: CQ4, CQ5
* Porosity Class
    * Rationale: Dense (XCT porosity under 0.5%) or porous (over 0.5%).
    * Connected Pattern: Explicit Typing
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx (XCT porosity column); the paper (the 0.5% line)
    * Competency Questions: CQ11, CQ16
* Test Method
    * Rationale: The test that made the numbers: Vickers hardness, X-ray CT, Archimedes weighing, tensile test.
    * Connected Pattern: Provenance, SOSA Observation (the procedure)
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx (test names in the headers)
    * Competency Questions: CQ5, CQ6, CQ9, CQ18
* Source
    * Rationale: Where a fact comes from: a dataset file, a section of the paper, or worked out by us.
    * Connected Pattern: Provenance
    * Source Dataset(s): not a column in any file; we add it
    * Competency Questions: CQ5, CQ14
* Measured Property
    * Rationale: The thing being measured, such as porosity, whichever test measured it.
    * Connected Pattern: SOSA Observation
    * Source Dataset(s): AlSi10Mg PSP feature table.xlsx (the headers)
    * Competency Questions: CQ6

# Link Names

Each link is read in the direction of the arrow. Every pattern keeps its own version of its links.

| Pattern | Link | From → To |
|---|---|---|
| Quantity | hasValue | Sample → Reported Value |
| Quantity | hasLabel | Reported Value → Label |
| Quantity | hasProcessParameter | Sample → Process Parameter |
| Quantity | hasParameterLabel | Process Parameter → Label |
| Aggregation | memberOf | Sample → Group |
| Aggregation | builtFrom | Reported Value → Raw Data |
| Aggregation | hasValue | Sample → Reported Value |
| Aggregation | hasLabel | Reported Value → Label |
| Aggregation | hasRawLabel | Raw Data → Label |
| Provenance | hasSource | Reported Value → Source |
| Provenance | recordedIn | Raw Data → Source |
| Provenance | measuredWith | Reported Value → Test Method |
| Provenance | testedWith | Sample → Test Method |
| Provenance | hasValue | Sample → Reported Value |
| Provenance | hasLabel | Reported Value → Label |
| Provenance | hasRawLabel | Raw Data → Label |
| Data Transformation | calculatedBy | Reported Value → Calculation |
| Data Transformation | hasLabel | Reported Value → Label |
| Data Transformation | usesAlgorithm | Calculation → Algorithm |
| Data Transformation | hasRawInput | Calculation → Raw Data |
| Data Transformation | hasParameterInput | Calculation → Process Parameter |
| Data Transformation | hasValueInput | Calculation → Reported Value |
| Data Transformation | hasRawLabel | Raw Data → Label |
| Data Transformation | hasParameterLabel | Process Parameter → Label |
| SOSA Observation | hasMeasuredProperty | Sample → Measured Property |
| SOSA Observation | hasLabel | Measured Property → Label |
| SOSA Observation | measuredWith | Measured Property → Test Method |
| SOSA Observation | hasValue | Measured Property → Reported Value |
| Explicit Typing | hasClass | Sample → Porosity Class |
