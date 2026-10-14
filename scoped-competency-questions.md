# Scoped Competency Questions

*L is a label (the kind of number, like hardness). G is a group (small or large hatch spacing). S is a sample, and A and B are two samples. M is a measurement method. X and Z are limits: X starts at 2 spreads and Z starts at 1 spread of the group, and both can be changed.*

**CQ1.** For a label L and a group G, which samples have a value that is more than the limit X away from the average of L in G? **[Label, hasLabel, Reported Value, hasValue, Sample, memberof, Group].**

**CQ2.** For a label L and a group G, bring out all the raw readings behind every value that is over the limit X, and show if each one was caused by one raw reading or by the whole sample.

*Follow-up query:* with the odd readings taken out, is the value  still over the limit X? If yes, the whole sample is the cause. If no, those readings are the cause. If the raw readings are missing, or the value can't be matched, the answer is "can't tell". **[Sample, Reported Value, hasValue, Label, hasLabel, memberof, Group, builtFrom, Raw Data].**

**CQ3.** For two samples A and B with label L, which Process parameter different?
*List version:* for a sample A and a process parameter P, which samples differ from A only in P, and did L change? **[Sample, Label, hasLabel, Reported Value, hasValue, Process Parameter, hasProcessParameter, memberof, Group].**

**CQ4.** For a label L, is it a setting, an observed value, calculated from settings, or calculated from observed data? If it is calculated, how is it calculated and from what?**[Label, hasLabel, calculatedBy, Calculation, Input].**

**CQ5.** For a value V, where did it come from: how was it made, which raw readings are behind it, which file are they in, and what test method was used? **[Reported Value, calculatedBy, Calculation, hasInput, Raw Data, hasSource, Source, measuredWith, Test Method].**

**CQ6.** Which properties are measured by more than one method, and for a sample S, what value does each method give and how far apart are they? **[Label, measuredWith, Test Method, Sample, hasMeasuredProperty, Measured Property, hasValue, Reported Value].**

**CQ7.** For a mechanical label L and a range of values, which samples are in the range, and what are their process parameters and structure values? **[Sample, hasValue, Reported Value, hasProcessParameter, Process Parameter].**

**CQ8.** For a sample S, how many raw readings are behind each of its values (per label), how many in total, and how many of them were used?**[Sample, hasValue, Reported Value, hasLabel, Label, builtForm, Raw Data].**

**CQ9.** For a measurement method M (such as X-ray CT), were the settings the same for all samples?**[Test Method, measuredWith, Sample, Settings, hasSettings].** 

**CQ10.** For a label L, which sample has the most raw readings behind its value? **[Sample, hasValue, Reported Value, hasLabel, Label, builtFrom, Raw Data].**

**CQ11.** Which samples share the same VED but have different MED (power divided by the square root of speed), and why (which input differs)? **[Sample, hasVale, Reported Value, hasLabel, Label, calculatedBy, Calculation, hasInput, Process Parameter].**

**CQ12.** Which pairs of samples differ in exactly one process parameter, where one is marked dense (XCT porosity under 0.5%) and the other porous (over 0.5%)? **[Sample, hasValue, Reported Value, hasLabel, Label, hasClass, Porosity Class, hasProcessParameter, Process Parameter].** 

**CQ13.** If a value of a sample S for a label L looks off, was it one reading or the whole sample, and is S also unusual in other labels? **[hasValue, Reported Value, hasLabel, Label, Sample].**

**CQ14.** For a sample S, what are all of its values, with their labels?
**[Sample, hasValue, Reported Value, hasLabel, Label]**

**CQ15.** Which values have no raw readings behind them?
**[Reported Value, builtFrom, Raw Data]**

**CQ16.** For a source S (a file in the dataset, or a section of the paper), which values come from it?
*Follow-up query:* which values come from the paper and not from the dataset?
**[Source, hasSource, Reported Value, hasLabel, Label]**

**CQ17.** If a raw reading or a process parameter changes, which values would be affected?
**[Raw Data, builtFrom, Reported Value, calculatedBy, Calculation, hasInput, Process Parameter]**

**CQ18.** For a group G, how many samples are dense and how many are porous?
**[Group, memberOf, Sample, hasClass, Porosity Class]**

**CQ19.** For a test method M, which labels does it give?
**[Test Method, measuredWith, Label]**


