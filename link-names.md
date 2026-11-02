# Link Names
 
Each link is read in the direction of the arrow. Every pattern keeps its own version of its links. A data link ends in a datatype (xsd:double) and holds a number.
 
| Pattern | Link | From → To | Type |
|---|---|---|---|
| Quantity | hasLabel | Reported Value → Label | object |
| Quantity | hasNumericValue | Reported Value → xsd:double | data |
| Quantity | hasParameterLabel | Process Parameter → Label | object |
| Quantity | hasParameterValue | Process Parameter → xsd:double | data |
| Quantity | hasProcessParameter | Sample → Process Parameter | object |
| Quantity | hasQuantityKind | Label → Quantity Kind | object |
| Quantity | hasUnit | Label → Unit | object |
| Quantity | hasValue | Sample → Reported Value | object |
| Aggregation | builtFrom | Reported Value → Raw Data | object |
| Aggregation | hasLabel | Reported Value → Label | object |
| Aggregation | hasNumericValue | Reported Value → xsd:double | data |
| Aggregation | hasRawLabel | Raw Data → Label | object |
| Aggregation | hasRawValue | Raw Data → xsd:double | data |
| Aggregation | hasValue | Sample → Reported Value | object |
| Aggregation | memberOf | Sample → Group | object |
| Provenance | hasLabel | Reported Value → Label | object |
| Provenance | hasRawLabel | Raw Data → Label | object |
| Provenance | hasSource | Reported Value → Source | object |
| Provenance | hasValue | Sample → Reported Value | object |
| Provenance | measuredWith | Reported Value → Test Method | object |
| Provenance | recordedIn | Raw Data → Source | object |
| Provenance | testedWith | Sample → Test Method | object |
| Data Transformation | calculatedBy | Reported Value → Calculation | object |
| Data Transformation | hasInput | Calculation → Label | object |
| Data Transformation | hasLabel | Reported Value → Label | object |
| Data Transformation | hasParameterInput | Calculation → Process Parameter | object |
| Data Transformation | hasParameterLabel | Process Parameter → Label | object |
| Data Transformation | hasRawInput | Calculation → Raw Data | object |
| Data Transformation | hasRawLabel | Raw Data → Label | object |
| Data Transformation | hasValueInput | Calculation → Reported Value | object |
| Data Transformation | usesAlgorithm | Calculation → Algorithm | object |
| SOSA Observation | hasLabel | Reported Value → Label | object |
| SOSA Observation | hasObservation | Sample → Observation | object |
| SOSA Observation | hasQuantityKind | Label → Quantity Kind | object |
| SOSA Observation | hasResult | Observation → Reported Value | object |
| SOSA Observation | observedQuantityKind | Observation → Quantity Kind | object |
| SOSA Observation | observedWith | Observation → Test Method | object |
| Explicit Typing | hasClass | Sample → Porosity Class | object |
| Explicit Typing | hasOrigin | Label → Value Origin | object |
