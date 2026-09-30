# Problem Statement

Every 3D printed testing specimen has a lot of data files which are then compiled into a master summary data file. But the information about individual data gets lost. Similarly, it loses where those came from, on average how many were taken, or if there were any outliers. Or for something like porosity, whether there are any big pores and very small pores or if all the pores were nearly similar, and how many big pores there are. Also, there is no way to tell by looking at the data which values are calculated and which are input or observed data.

Same thing happens with the energy density values in this dataset. They are not measured at all, they are calculated from the processing parameters using a formula. But sitting next to the measured values in the spreadsheet, there is no way to tell that apart either.

In this dataset, which is similar to most 3D printed specimen datasets, the summary spreadsheet does not have all the information. And the sources are varied and disconnected enough to make it harder to understand. This makes it easy to find the result but makes it harder to ask questions. This is the problem this project will try to solve.

This project builds a structured representation that keeps those connections intact, so the raw measurements, the instruments, and the calculations behind every summary value stay traceable.
