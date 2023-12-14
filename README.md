# GEOG5995---Final-Project

This project explores the relationship between the Index of Multiple Deprivation [IMD] scores and reoffending rates by geographical regions in England (Department for Levelling Up, Housing and Communities, 2020; Ministry of Justice [MoJ], 2022). By examining the possible factors which contribute to reoffending behaviour, preventative measures can be uncovered and used for the public good. This research is especially important in current times, as there is a UK wide issue of prison overcrowding (Foster and Anderson, 2023). Prisons and England and Wales are struggling to cope with the offender population, reporting extraordinary figures this year which are predicted to only increase (Beard, 2023; MoJ, 2023). Consequences of such are drastic; the safety of prisoners is dramatically reduced, with levels of violence rising (Taylor, 2023). Often a product of the poor environment, a lack of physical space and diminished out of cell activities due to understaffing only heighten such issues (Taylor, 2023). For this reason, it is more important, now than ever, to uncover the determining factors of reoffending. 
 
In regard to the relationship between crime and poverty, there is a large amount of literature which corroborates the hypothesis that offending behaviour is linked to deprivation (e.g. Rhudy and Schuerman, 2009; Weatherburn and Lind, 1998), and also reoffending (Hay and Forrest, 2009). Linking these correlations to the wealth and deprivation disparities between the North and South of England is essential in understanding reoffending in local contexts. Analysing the variation in criminal behaviour between regions with differing IMD scores will allow policymakers to focus on appropriate resource allocation, improving both life quality and limiting persistent offending more effectively in such areas. 
 
Within the GitHub repository, there are three separate datasets. The first dataset ‘Proven Reoffending Overview’, published by the MoJ (extracted from the Police National Computer), was used for the data relating to reoffending. It had a geographical data column, showing the number of offenders in each region. However, it had no actual spatial data/polygon points. The data is aggregated by cohort. There are quarterly cohorts, where offenders who were released from custody, received a non-custodial conviction at court, or received a caution within a three-month period of each year between 2008-2020 were recorded. A proven reoffence, in this dataset, is defined as any offence committed in a one-year follow-up period or a further six-month waiting period (to allow time for cases to progress through the courts). This particular dataset was chosen as its geographical element was able to be matched to another spatial dataset. Initially, the analysis was attempted on ‘Geographical data tool, April 2019 to March 2020’, which had more detailed data. It included variables such as ethnicity, which would have been useful for the regression modelling. However, the geographical data related to probation areas and could not be found in any spatial dataset with such polygon points.
 
The second dataset used was ‘English IMD 2019’, published by the Department for Levelling Up, Housing and Communities, was used for IMD scores. IMD is ‘the official measure of relative deprivation for small areas in England; the IMD combines information from the seven domains to produce an overall relative measure of deprivation. The domains are combined using the following weights: Income Deprivation (22.5%), Employment Deprivation (22.5%), Education, Skills, and Training Deprivation (13.5%), Health Deprivation and Disability (13.5%), Crime (9.3%), Barriers to Housing and Services (9.3%), Living Environment Deprivation (9.3%)’ (Ministry of Housing, Communities and Local Government, 2019: p5). IMD scores, which is the measure used within this research, ‘relate to a proportion of the relevant population experiencing that type of deprivation’ (Ministry of Housing, Communities and Local Government, 2019: p19). 
 
The final dataset imported was ‘2011 Census Geography boundaries (Regions)’, published by the Office for National Statistics, was used for the regional data points. As the spatial data in the IMD dataset was at an LSOA level, another spatial dataset was needed to be able to plot a choropleth map for the regions set out by the reoffender’s dataset.
 
Links to the webpages for the datasets:
Proven reoffending statistics: January to March 2020 - GOV.UK 
Index of Multiple Deprivation (IMD) | CDRC Data 
2011 Census Geography boundaries (Regions) - Dataset - UK Data Service CKAN 
 
Within this project, the code aims to clean the data appropriately, creating visualisations along the way to aid in exploration of the data. It also aims to create a regression model, to help understand the relationship between reoffending and IMD scores. As well as generating two final data visualisations, one spatial (two choropleth maps, side by side, showing both the reoffending rate and average IMD score for each region) and one non-spatial (a scatterplot of the reoffending rate by average IMD score, with an added key for regional information).
 
Overall, the analysis shows us that there is a relationship between reoffending and IMD scores regionally. The more deprivation an area has, the more likely it is to have a higher rate of reoffending. It was found that the North East had both the highest reoffending rate, and also the highest IMD score. In comparison, the South East has the lowest IMD score and lowest reoffending rate. The results of this analysis agree with the large majority of the literature which suggests a correlation between poverty and crime.
 
Note: in order for the notebook to work correctly, the code must be run in order. As the datasets are so large, if certain actions are run before they are clipped, it causes the kernel to die. Please also change the file paths to your own desktop when loading the data. 
 
References:
 
Beard, J. (2023). What is the Government doing to reduce pressure on prison capacity? London: UK Parliament. 
 
Department for Levelling Up, Housing and Communities. (2020). English IMD 2019. [Online]. [Accessed 10 November 2023]. Available from: https://data.cdrc.ac.uk/ 
 
Hay, C. and Forrest, W. (2009). The implications of family poverty for a pattern of persistent offending. In: Savage, E. ed. The development of persistent criminality. Oxford: Oxford University Press, pp.54-70.
 
Taylor, C. (2023). Why the prison population crisis is everyone's concern. London: HM Inspectorate of Prisons.
 
Foster, R. and Anderson, K. (2023). Longer sentences? Overcrowded UK prisons are already failing society. The Conversation. [Online]. 7 November. [5th December 2023]. Available from: https://theconversation.com/ 
 
Ministry of Housing, Communities and Local Government. (2019). The English Indices of Deprivation 2019. London: Ministry of Housing, Communities and Local Government. 
 
Ministry of Justice. (2023). Prison Population Projections 2022 to 2027, England and Wales. London: National Statistics.
 
Ministry of Justice. (2022). Proven Reoffending Overview data tool, April 2019 to March 2020. [Online]. [Accessed 7 November 2023]. Available from: https://www.gov.uk/
 
Office for National Statistics. (2020). 2011 Census Geography boundaries (Regions). [Online]. [Accessed 20 November 2023]. Available from: https://statistics.ukdataservice.ac.uk/ 
 
Rhudy, K. and Schuerman, J. (2009). Breaking the cycle of offending and poverty: A symposium on the intersection of juvenile justice and poverty. Georgetown Journal on Poverty Law & Policy. 16, pp. 461-470.

Weatherburn, D. and Lind, B. (1998). Poverty, parenting, peers and crime-prone neighbourhoods. In: Trends and Issues in Crime and Criminal Justice, No. 85. Canberra: Australian Institute of Criminology.
