# Axioms
* Calculation: `usesAlgorithm exactly 1 Algorithm`
* Label: `hasOrigin exactly 1 ValueOrigin`
* Label: `hasQuantityKind exactly 1 QuantityKind`
* Observation: `hasResult exactly 1 ReportedValue`
* Observation: `observedProperty exactly 1 QuantityKind`
* Observation: `observedWith exactly 1 TestMethod`
* ProcessParameter: `hasParameterLabel exactly 1 Label`
* QuantityValue: `hasNumericValue exactly 1 xsd:double`
* QuantityValue: `hasUnit max 1 Unit`
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
* Sample: `testedWith some TestMethod`


## Subclass axioms
 
* ProcessParameter SubClassOf QuantityValue
* RawData SubClassOf QuantityValue
* ReportedValue SubClassOf QuantityValue

## Property chain axioms
 
* `hasObservation o observedWith` implies `testedWith`

## Controlled vocabularies
* Porosity Class: dense, porous
* Value Origin: set, measured, calculated
* Group: small (samples 1 to 32), large (samples 33 to 60)
* Test Method: Vickers hardness, X-ray CT, Archimedes weighing, tensile test
* Source: dataset file, paper section, worked out
* Quantity Kind: reused from QUDT 
* Unit: reused from QUDT 
