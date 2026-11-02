# Axioms (combined ontology)
* Calculation: `usesAlgorithm exactly 1 Algorithm`
* Label: `hasOrigin exactly 1 ValueOrigin`
* Label: `hasQuantityKind exactly 1 QuantityKind`
* Label: `hasUnit max 1 Unit`
* Observation: `hasResult exactly 1 ReportedValue`
* Observation: `observedQuantityKind exactly 1 QuantityKind`
* Observation: `observedWith exactly 1 TestMethod`
* ProcessParameter: `hasParameterLabel exactly 1 Label`
* ProcessParameter: `hasParameterValue exactly 1 xsd:double`
* RawData: `hasRawLabel min 1 Label`
* RawData: `hasRawValue exactly 1 xsd:double`
* RawData: `recordedIn exactly 1 Source`
* ReportedValue: `calculatedBy max 1 Calculation`
* ReportedValue: `hasLabel exactly 1 Label`
* ReportedValue: `hasNumericValue exactly 1 xsd:double`
* ReportedValue: `hasSource min 1 Source`
* ReportedValue: `measuredWith max 1 TestMethod`
* Sample: `hasClass max 1 PorosityClass`
* Sample: `hasObservation min 1 Observation`
* Sample: `hasProcessParameter min 1 ProcessParameter`
* Sample: `hasValue min 1 ReportedValue`
* Sample: `memberOf exactly 1 Group`
* Sample: `testedWith some TestMethod`
## Property chain axioms
 
* `hasObservation o observedWith` implies `testedWith`
