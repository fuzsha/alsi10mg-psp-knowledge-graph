# Axioms (combined ontology)

* Calculation: `usesAlgorithm exactly 1 Algorithm`
* Label: `measuresProperty exactly 1 MeasuredProperty`
* Observation: `hasResult exactly 1 ReportedValue`
* Observation: `observedProperty exactly 1 MeasuredProperty`
* Observation: `observedWith exactly 1 TestMethod`
* ProcessParameter: `hasParameterLabel exactly 1 Label`
* RawData: `hasRawLabel min 1 Label`
* RawData: `recordedIn exactly 1 Source`
* ReportedValue: `calculatedBy max 1 Calculation`
* ReportedValue: `hasLabel exactly 1 Label`
* ReportedValue: `hasSource min 1 Source`
* ReportedValue: `measuredWith max 1 TestMethod`
* Sample: `hasClass max 1 PorosityClass`
* Sample: `hasObservation min 1 Observation`
* Sample: `hasProcessParameter min 1 ProcessParameter`
* Sample: `hasValue min 1 ReportedValue`
* Sample: `memberOf exactly 1 Group`
* Sample: `testedWith min 1 TestMethod`
