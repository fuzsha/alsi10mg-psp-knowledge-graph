# Scoped Competency Questions


## Master and Supporting

**CQ1.** What is the reason for a higher standard deviation in any data? Was it because of one data point or one sample?
*(originally Q2 and Q14 merged, since both ask the same thing)*

**CQ2.** Can the change in observed data be tracked to any process parameter?
*(originally Q3)*

**CQ3.** Which data are calculated from processing parameters, which are just observed data, and which are calculated from observed data?
*(originally Q5)*

**CQ4.** What is the source of each data point, and what is the chain of data? (Where is each data point coming from, and what testing method was used to get it?)
*(originally Q6)*

**CQ5.** Which data has been measured using multiple methods, and do the different methods give similar results?
*(originally Q7 and Q8 merged, since Q8 is the natural follow-up to Q7)*

**CQ6.** For mechanical property data, for a range of results, which parameter or structural property do they come from?
*(originally Q9)*

**CQ7.** How much data is used to get into the master table?
*(originally Q10)*

**CQ8.** Which samples had the same processing input but ended up in a different structural regime?
*(originally Q12)*

**CQ9.** Were all the observation/measurement settings (such as X-ray CT) kept the same?
*(originally Q17)*

**CQ10.** Which sample had the most raw data?
*(originally the first half of Q21)*

## Rescoped


**CQ11.** *(originally Q11)* Which samples share the same VED but have different MVED, and why (which input differs)?

**CQ12.** *(originally Q18)* If a sample's data looks off, can we tell whether the problem came from the sample itself or from how it was measured?

**CQ13.** *(originally Q19)* Retrieve and compare mechanical property values for small vs. large hatch spacing samples.

**CQ14.** *(originally Q23)* Retrieve the stored yield-point value for each sample and compare across samples.

## Out of Scope

**Q1.** Besides process parameters, what changes PV process features?
This is asking *why* PV changes, not what PV is. The graph can show PV and how it's calculated, but figuring out what else might be influencing it is a physics question, not something to look up.

**Q4.** Why is there a difference between the average and root mean square values for surface roughness?
This is just math/stats the difference between a mean and an RMS is a known thing, not something the dataset or graph explains. 

**Q13.** Why do we need process features when input parameters are already there? Do they do the same job?
This is really asking "why did the researchers bother calculating VED/MVED instead of just using power and speed directly" that's a question about their methodology and reasoning, not something the data can answer.

**Q15.** Does the pore count matter as much as pore volume?
This is asking which one is a better predictor that's the kind of thing the original paper's machine learning model figured out through analysis. 
**Q16.** Is the biggest pore a better predictor for failure than average pore size?
Same issue as Q15 this is a prediction/importance question, not a lookup question.

**Q20.** How does one structural property change another structural property, and can this be found in the data?
This is asking for a cause-and-effect relationship between two structural features. That's exactly what the paper's ML analysis was built to find  it's not something that can be just pull out of the graph.

**Q21 (second half).** Is there any relation between the sample with the most raw data and its process parameters?
The "which sample had the most raw data" part is fine (that's CQ10), but asking if that's *related* to its process parameters is asking for a cause-and-effect explanation, which isn't a lookup.

**Q22.** For finding Young's modulus, how much fitting is needed on the stress-strain curve?
This is a methods question about how the curve-fitting was done  .
