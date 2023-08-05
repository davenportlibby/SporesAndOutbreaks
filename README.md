# Davenport et al. study on parasite environmental transmission stage concentration and disease outbreaks
---

The files include all the data and code used to create the figures in the Davenport et al. manuscript. Data collection was led by Elizabeth Davenport and supported by Marcin Dziuba, Logan Jacobson, Siobhan Calhoun, and Kira Monell. Figures were created by Elizabeth Davenport and Meghan Duffy of the University of Michigan. 

## Description of the data and file structure

There are three main folders in the zip file:
1. scripts: this contains the code used to create figures.

2. data: this contains the data collected during the study.

3. figures: this is the folder where plots will be saved from the output of the R markdown files.

## Sharing/Access information

During the review process, data and code were posted at:
(https://github.com/davenportlibby/SporesAndOutbreaks)

# Spore Concentrations and Outbreak Data
Data and code for 2021 field study led by Elizabeth Davenport

Citation: How does parasite environmental transmission stage concentration change before, during, and after outbreaks?

Authors: Elizabeth S. Davenport 1*, Marcin K. Dziuba 1, Logan E. Jacobson 1, Siobhan K. Calhoun 1, Kira J. Monell 1, and Meghan A. Duffy 1
        1 Department of Ecology & Evolutionary Biology, University of Michigan, Ann Arbor, MI 48109, USA

Contact: * Author responsible for writing code related to analyses and figures: davenpe@umich.edu
         
Date: August 2023

_______________________________________________________________________________________________________________

DATA

AvgDaysBetweenSporeIncreaseAndOutbreakStart.csv: this data file contains the number of days between the initial spore increase and the beginning of the disease outbreak (defined as the first sampling date when percent infection reached 1% or higher). Negative values describe spore concentrations increasing before outbreaks begin. Data are shown for the 13 lake*parasite outbreaks described in the manuscript. Lake = name of the lake sampled. HostSpecies = name of the host species experiencing the outbreak. Parasite = name of the parasite species causing the outbreak. DaysBetweenSporeIncreaseAndOutbreakStart = number of days between the initial spore increase and the beginning of the outbreak.

DaysBetweenPeaks.csv: this data file contains the number of days between the peaks in spore concentration and the peaks in disease outbreaks. Positive values describe spore concentration peaking after disease outbreaks peak. Negative values describe spore concentrations peaking before outbreaks peak. Parasite = name of the parasite species causing the outbreak. Lake = name of the lake sampled. DaysBetweenPeaks = the number of days between the peak in spore concentration and the peak in infections.

Walsh_Mean_Metsch_PercentInfected.csv: this data file contains the mean spore concentration of Metschnikowia bicuspidata and percent infection of Daphnia dentifera by Metschnikowia bicuspidata in Walsh Lake from June 14, 2021 to November 12, 2021. datetime = sampling dates. Lake = name of lake sampled. Mean = mean spore concentration of Metschnikowia bicuspidata in spores per L. PercentInfected = percentage of the Daphnia dentifera host population infected with Metschnikowia bicuspidata.

Metsch_Mean_Spores_Outbreak.csv: this data file contains the mean spore concentration of Metschnikowia bicuspidata in all six lakes that were sampled, regardless of outbreak occurrence, June 2021 to November 2021. datetime = sampling dates. Lake = name of lakes sampled. Mean = mean spore concentration of Metschnikowia bicuspidata in spores per L. Outbreak = yes means that an outbreak of Metschnikowia bicuspidata occurred in the lake; no means that an outbreak of Metschnikowia bicuspidata did not occur in the lake.

Pasteuria_Mean_Spores_and_Percent_Infected_Outbreak.csv: this data file contains the mean spore concentration of Pasteuria ramosa and percent infection of multiple zooplankton hosts. If fewer than 20 individuals of a host species were observed in a field sample, percent infection was not recorded for that species and is either NA or blank. datetime = sampling dates. Lake = name of lake sampled. Mean = mean spore concentration of Pasteuria ramosa in spores per L. Dent_Per_Inf = percent infection of Daphnia dentifera by Pasteuria ramosa. Retro_Per_Inf = percent infection of Daphnia rectrocurva by Pasteuria ramosa. Cerio_Per_Inf = percent infection of Ceriodaphnia dubia by Pasteuria ramosa. Parv_Per_Inf = percent infection of Daphnia parvula by Pasteuria ramosa. Outbreak = yes means that an outbreak of Pasteuria ramosa occurred in the lake; no means that an outbreak of Pasteuria ramosa did not occur in the lake. 

Brood_Mean_Spores_and_Percent_Infected_OutbreakSize.csv: this data file contains the mean spore concentration of Blastulidium paedophthorum and percent infection of multiple zooplankton hosts. If fewer than 20 individuals of a host species were observed in a field sample, percent infection was not recorded for that species and is either NA or blank. datetime = sampling dates. Lake = name of lake sampled. Mean = mean spore concentration of Blastulidium paedophthorum in spores per L. Dent_Per_Inf = percent infection of Daphnia dentifera by Blastulidium paedophthorum. Cerio_Per_Inf = percent infection of Ceriodaphnia dubia by Blastulidium paedophthorum. Dubia_Per_Inf = percent infection of Daphnia dubia by Blastulidium paedophthorum. Retro_Per_Inf = percent infection of Daphnia rectrocurva by Blastulidium paedophthorum. Pulic_Per_Inf = percent infection of Daphnia pulicaria by Blastulidium paedophthorum. Parv_Per_Inf = percent infection of Daphnia parvula by Blastulidium paedophthorum. Outbreak = yes means that an outbreak of Blastulidium paedophthorum occurred in the lake; no means that an outbreak of Blastulidium paedophthorum did not occur in the lake.

BroodOutbreakMeans.csv: this file contains the mean spore concentration of Blastulidium paedophthorum for all six lakes and documents the occurrence of an outbreak. Lake = name of lake sampled. Parasite = Blastulidium paedophthorum. LogMean = Log of the mean spore concentration plus 1. RawMean = the raw spore concentration data. SD = standard deviation of the spore concentration. Outbreak = "yes" means an outbreak occurred in the lake, "no" means there was not an outbreak in the lake.

BroodOutbreakMeanStats.csv: this file contains the mean spore concentration of Blastulidium paedophthorum in lakes that had outbreaks and lakes that did not have outbreaks. Parasite = Blastulidium paedophthorum. NoOutbreakMean = mean spore concentration in lakes without outbreaks. OutbreakMean = mean spore concentration in lakes with outbreaks.

MicG_Mean_Spores_and_Percent_Infected_OutbreakSize.csv: this data file contains the mean spore concentration of Ordospora pajunii and percent infection of multiple zooplankton hosts. If fewer than 20 individuals of a host species were observed in a field sample, percent infection was not recorded for that species and is either NA or blank. datetime = sampling dates. Lake = name of lake sampled. Mean = mean spore concentration of Ordospora pajunii in spores per L. Dent_Per_Inf = percent infection of Daphnia dentifera by Ordospora pajunii. Parv_Per_Inf = percent infection of Daphnia parvula by Ordospora pajunii. Ambig_Per_Inf = percent infection of Daphnia ambigua by Ordospora pajunii. Cerio_Per_Inf = percent infection of Ceriodaphnia dubia by Ordospora pajunii. OutbreakSize = relative size of Ordospora pajunii outbreaks (medium = 15-25% of host population infected; large = over 25% of host population infected). Outbreak = yes means that an outbreak of Ordospora pajunii occurred in the lake; no means that an outbreak of Ordospora pajunii did not occur in the lake. 

Spiro_Mean_Spores_and_Percent_Infected.csv: this data file contains the mean spore concentration of Spirobacillus cienkowskii and percent infection of multiple zooplankton hosts. If fewer than 20 individuals of a host species were observed in a field sample, percent infection was not recorded for that species and is either NA or blank. datetime = sampling dates. Lake = name of lake sampled. Mean = mean spore concentration of Spirobacillus cienkowskii in spores per L. dent.perinf = percent infection of Daphnia dentifera by Spirobacillus cienkowskii. dub.perinf = percent infection of Daphnia dubia by Spirobacillus cienkowskii. mend.perinf = percent infection of Daphnia mendotae by Spirobacillus cienkowskii. pulic.perinf = percent infection of Daphnia pulicaria by Spirobacillus cienkowskii. retro.perinf = percent infection of Daphnia retrocurva. cerio.perinf = percent infection of Ceriodaphnia dubia by Spirobacillus cienkowskii. ambig.perinf = percent infection of Daphnia ambigua by Spirobacillus cienkowskii. parv.perinf = percent infection of Daphnia parvula by Spirobacillus cienkowskii.

LakeSporeMeans.csv: this data file contains the mean spore concentration over the entire sampling season for all six lakes. Lake = name of lake sampled. Parasite = parasite species. Mean = log of the mean spore concentration + 1 for the entire sampling period. SD = standard deviation of the mean spore concentration. Outbreak = "yes" means an outbreak occurred in the lake, "no" means there was not an outbreak in the lake.

Clean_Data_2021_Lakes_All_Host_Densities.csv: this file contains host density, total number of hosts, and infection prevalence. If fewer than 20 individuals of a host species were observed in a field sample, infection prevalence was not recorded for that species and is either NA or blank. Date, Julian.Day, Julian = sampling dates. Lake = name of lake sampled. Host.Species = name of the host species (ambigua = Daphnia ambigua; ceriodaphnia = Ceriodaphnia dubia; dentifera = Daphnia dentifera; dubia = Daphnia dubia; mendotae = Daphnia mendotae; pulicaria = Daphnia pulicaria; parvula = Daphnia parvula). Total = total number of individuals. Uninfected.Adult, Uninfected.Juv, Uninfected.Males = number of uninfected adults, juveniles, and males respectively. All columns ending in .inf = number of individuals infected by each parasite species (pasteuria = Pasteuria ramosa; metsch = Metschnikowia bicuspidata, spiro = Spirobacillus cienkowskii; brood = Blastulidium paedophthorum; larssonia, spider, gurleya, caullerya, and coke were not included in our spore sampling study). All columns ending in .prev = infection prevalence of each parasite species. All columns ending in .inf.density = infected host density organized by each parasite species. All columns ending in .density = host density organized by each host species.

Brood_Density_PercentInfection.csv: this file contains host density for host species that experienced an outbreak of B. paedophthorum. The file also includes percent infection and environmental mean B. paedophthorum spore concentration data. If fewer than 20 individuals of a host species were observed in a field sample, infection prevalence was not recorded for that species and is either NA or blank. All columns ending in .PerInf = percent infection for B. paedophthorum organized by host species. All columns ending in .density = host density organized by each host species. datetime = sampling dates. Lake = name of lake sampled. MeanSpore = mean B. paedophthorum spore concentration.

MicG_Density_PercentInfection.csv: this file contains host density for host species that experienced an outbreak of Ordospora pajunii. The file also includes percent infection and environmental mean O. pajunii spore concentration data. If fewer than 20 individuals of a host species were observed in a field sample, infection prevalence was not recorded for that species and is either NA or blank. All columns ending in .PerInf = percent infection for O. pajunii organized by host species. All columns ending in .density = host density organized by each host species. datetime = sampling dates. Lake = name of lake sampled. MeanSpore = mean O. pajunii spore concentration.

Pasteuria_density_percentinfection.csv: this file contains host density for host species that experienced an outbreak of Pasteuria ramosa. The file also includes percent infection and environmental mean P. ramosa spore concentration data. If fewer than 20 individuals of a host species were observed in a field sample, infection prevalence was not recorded for that species and is either NA or blank. All columns ending in .PerInf = percent infection for P. ramosa organized by host species. All columns ending in .density = host density organized by each host species. datetime = sampling dates. Lake = name of lake sampled. MeanSpore = mean P. ramosa spore concentration.

Walsh_Metsch_DentiferaDensity.csv: this file contains host density for Daphnia dentifera that experienced an outbreak of Metschnikowia bicuspidata in Walsh Lake. The file also includes percent infection and environmental mean M. bicuspidata spore concentration data. datetime = sampling dates. Lake = Walsh Lake. Mean = mean M. bicuspidata spore concentration. PercentInfected = percent of the D. dentifera population infected with M. bicuspidata. Dent.density = total density of D. dentifera.

SporeConcentrationBeginningVersusEnd.csv: this data file contains spore concentrations at the beginning of disease outbreaks and at the end of disease outbreaks. Lake = name of lake sampled. HostSpecies = host species experiencing an outbreak. Parasite = parasite species. Date_outbreak_reached_1% = the date that at least one percent of the host population was infected. SporeConcentration_OutbreakStart = the mean spore concentration on the sampling date that the outbreak began. Date_Outbreak_Ends = the date that no infections were observed or the end of the sampling season. SporeConcentration_OutbreakEnds = mean spore concentration on the sampling date when the outbreak ended. Change_in_Spore_Concentration = change in mean spore concentration from the beginning of the outbreak to the end of the outbreak.

SporeConcentrationBeginningVersusEndFigure.csv: this data file contains spore concentrations at the beginning of disease outbreaks and at the end of disease outbreaks. Lake = name of lake sampled. HostSpecies = host species experiencing an outbreak. Parasite = parasite species. Date = sampling date when the outbreak either started or ended. SporeConcentration = mean spore concentration. LogSporeConcentrationPlus1 = log of the mean spore concentration plus one. OutbreakStatus = the outbreak is either starting or ending. OutbreakID = numbering the outbreaks to group the starting and ending spore concentrations together.



_______________________________________________________________________________________________________________
