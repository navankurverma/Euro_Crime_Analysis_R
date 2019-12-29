# Europe Crime Analysis in R

Use this [link](https://navankurverma.github.io/Euro_Crime_Analysis_R/Euro_Crime_Analysis.html) to see the markdown file alongwith code and output.

I used data from Eurostat and CSO Ireland website (links to datasets are present in above link), to find out key points in data and visualize data such that in single graphics most of the data could be represented.

I have used below R packages in this reop:
1. rio - for importing the datasets
2. tidyverse (ggplot2, dplyr, tibble) - for manipulation and visualisation of data
3. gganimate - for animating the visual output
4. gifski, png - dependencies of gganimate

### Phase 1

##### Data Description
The Eurostat crime dataset records offences (values per hundred thousand in-habitants) by 13 offence categories in 41 European Countries from year 2008 to 2017. [link for further description](https://ec.europa.eu/eurostat/cache/metadata/en/crim_off_cat_esms.htm)

<details>
  <summary>13 Offence categories</summary>
  
  1. Intentional homicide
  2. Attempted intentional homicide
  3. Assault
  4. Kidnapping
  5. Sexual violence
  6. Rape
  7. Sexual assault
  8. Robbery
  9. Burglary
  10. Burglary of private residential premises
  11. Theft
  12. Theft of a motorized land vehicle
  13. Unlawful acts involving controlled drugs or precursors
</details>

<details>
  <summary>41 Countries</summary>
  
1. Belgium
2. Bulgaria
3. Czechia
4. Denmark
5. Germany (until 1990 former territory of the FRG)
6. Estonia
7. Ireland
8. Greece
9. Spain
10. France
11. Croatia
12. Italy
13. Cyprus
14. Latvia
15. Lithuania
16. Luxembourg
17. Hungary
18. Malta
19. Netherlands
20. Austria
21. Poland
22. Portugal
23. Romania
24. Slovenia
25. Slovakia
26. Finland
27. Sweden
28. England and Wales
29. Scotland
30. Northern Ireland (UK)
31. Iceland
32. Liechtenstein
33. Norway
34. Switzerland
35. Montenegro
36. North Macedonia
37. Albania
38. Serbia
39. Turkey
40. Bosnia and Herzegovina
41. Kosovo (under United Nations Security Council Resolution 1244/99)
</details>

##### Data Visualization
I have used Bar charts as basic structure for graphical represenation of data using RStudio, `ggplot2` package is used to define this basic structure. And for better visualisation over the whole period of time, I've also used `gganimate` package, to animate bar chart to change for every year available.
