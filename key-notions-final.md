# Key Notions
 
* Sample
    * Rationale: One printed sample, with its own printing settings. Every number belongs to one sample.
    * Competency Questions: CQ1, CQ2, CQ3, CQ6, CQ7, CQ8, CQ9, CQ10, CQ11, CQ12, CQ13, CQ14, CQ18
* Group
    * Rationale: A set of samples with the same hatch spacing: small (samples 1 to 32) or large (33 to 60). Samples are compared inside their own group.
    * Competency Questions: CQ1, CQ2, CQ3, CQ13, CQ18
* Reported Value
    * Rationale: A number that came out of a measurement or a calculation, for one sample: hardness, porosity, or a calculated process feature such as VED, MED, LED. Its label has the origin "measured" or "calculated". Its number is stored with `hasNumericValue`. Settings and results can sit in the same table or file, so the file does not tell them apart; the origin does.
    * Competency Questions: CQ1, CQ2, CQ3, CQ4, CQ5, CQ6, CQ7, CQ8, CQ10, CQ11, CQ12, CQ13, CQ14, CQ15, CQ16, CQ17, CQ19
* Process Parameter
    * Rationale: A setting that the researchers chose and typed in before printing: laser power, scan speed, layer thickness, hatch spacing. It was not measured and not calculated. Its label has the origin "set". Its number is stored with `hasParameterValue`.
    * Competency Questions: CQ3, CQ4, CQ7, CQ9, CQ11, CQ12, CQ17
* Label
    * Rationale: The named field of a number in the dataset, such as "Laser power", "VED", "Vickers hardness" or "Density (Archimedes)". It only names the field. What it measures, its unit, and how it was obtained are kept in the three notions below.
    * Competency Questions: CQ1, CQ2, CQ3, CQ4, CQ6, CQ7, CQ8, CQ10, CQ11, CQ12, CQ13, CQ14, CQ16, CQ19
* Quantity Kind
    * Rationale: What physical thing the label is about, such as density, hardness or power. Two labels can have the same quantity kind (density from Archimedes and density from X-ray CT). Aligned to QUDT QuantityKind, like the MODL Quantity pattern (`hasQuantityKind`). Replaces Measured Property.
    * Competency Questions: CQ6
* Unit
    * Rationale: The unit of a label, such as W, mm/s, mm or %. Aligned to QUDT Unit, so we reuse QUDT units and do not define our own. Needed to compare two values of the same quantity kind.
    * Competency Questions: CQ6
* Value Origin
    * Rationale: How the numbers of a label were obtained: set (typed in by the researchers), measured (from a test), or calculated (from other numbers). It is a small fixed set of types, like Porosity Class.
    * Competency Questions: CQ4
* Raw Data
    * Rationale: One single reading behind a final number: one hardness dent, one pore, one weighing. Its number is stored with `hasRawValue`.
    * Competency Questions: CQ2, CQ5, CQ8, CQ10, CQ13, CQ15, CQ17
* Calculation
    * Rationale: The step that makes a final number from readings, settings or other values (an average, a formula).
    * Competency Questions: CQ4, CQ5, CQ11, CQ17
* Algorithm
    * Rationale: The formula or method a calculation follows, such as VED = P / (v x h x t) or the average of 10 readings.
    * Competency Questions: CQ4
* Porosity Class
    * Rationale: Dense (XCT porosity under 0.5%) or porous (over 0.5%).
    * Competency Questions: CQ12, CQ18
* Test Method
    * Rationale: The test that made the numbers: Vickers hardness, X-ray CT, Archimedes weighing, tensile test.
    * Competency Questions: CQ5, CQ6, CQ9, CQ19
* Source
    * Rationale: Where a fact comes from: a dataset file, a section of the paper, or worked out.
    * Competency Questions: CQ5, CQ16
* Observation
    * Rationale: One measurement event on one sample: which quantity kind was looked at, which test method was used, and which reported value came out. It lets us put two results for the same quantity kind side by side.
    * Competency Questions: CQ6
 
