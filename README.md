# Symbiodiniaeae_Pump_Iron

## Welcome to the github page for the paper "Endosymbiotic dinoflagellates pump iron: Differences in iron and other trace metal needs among the Symbiodiniaceae" - Hannah Reich, Irene Rodriguez, Todd LaJeunesse, Tung-Yuan Ho. (In Press; Coral Reefs). 

### Below, please a brief overview of each file and the abstract. Feel free to reach out w/ questions anytime via email: hgreich16 [at] gmail [dot] com

## General remarks 
**Species Abbreviations**: min/bmin = Breviolum minutum; psyg/psygmo/bpsyg = Breviolum psygmophilum; vor/evor = Effrenium votatum; smic = Symbiodinium microagriaticum; necro/snec = Symbiodinium necroappetens

**Iron concentration abbreviations** The data files use the total desolved iron concentrations throughout. In the paper/figures, the treatments are referred to by their bioavailable iron concentrations (pM Fe') which makes the study comparable to others. Following the addition of EDTA, the "estimated inorganic concentrations of 0, 250, 500, and 1250 pM Fe' represented the bioavailable fractions and correspond to the total dissolved iron concentrations 0, 50, 100, and 250 nM Fe, respectively (Rodriguez et al. 2016; Rodriguez and Ho 2017,2018). Hereafter, the iron treatments will be referred to as starvation (0 pM Fe'), low iron (250 pM Fe'), intermediate iron (500 pM Fe') and replete iron (1,250 pM Fe')."

Many of these figures were coded back in the good 'ol days where loading cowplot would automatically set plot theme. Note: As of version 1.0.0, cowplot does not change the default ggplot2 theme anymore. To recover the previous behavior, execute: theme_set(theme_cowplot())

## File overview
**raw_cell_count_tracker** Excel file with raw cell count data (batch sheet). Cell densities were calculated with a beckman coulter counter for 5 Symbiodiniaceae species exposed to 4 iron concentrations. The innoculation density sheet includes cell density info for stock cultures

**fig_2_stats.xlsx** Excel file of cell density and stdev of cultures exposed to four iron concentrations (averages and stdev are from raw cell count tracker file).

**fig_2_cell_density_.Rmd** Rmarkdown file of cell density figure (fig 2) and corresponding statistics. Calls upon the fig_2_stats excel file. 

**fig_3_specific_growth.xlsx** Excel file with sheets including average specific growth (used for R), and the (raw) calculation for each species. 

**fig_3_specific_growth.Rmd** corresponding Rmarkdown file for specific growth figure (Fig 3)

**metal_data.xlsx** Results from HR-ICPMS elemental analysis of Symbiobiodiniaceae species exposed to different iron concentrations.

**fig_4-5_S1_S2_metal_figs_REVISED_112019.Rmd** Metal content, uptake, & efficiency figures (4, 5, S1, S2) and bivariate statsitics. Calls upon metal_data excel file. 

**fig_6_pca.Rmd** Multivariate analysis of Symbiodiniaceae trace metal content (Fig 6). Calls upon metal_data excel file. This PCA uses features from the FactoMineR and ggplot2 packages (so shape can demark one factor and color another factor, see lines 115-130).

**fig_s3_allalgae_growthcomparison_DATA.xlsx** Excel file for Fig S3. Compares specific growth rate of Symbiodiniaceae at different bioavailable iron concentrations to other phytoplankton. These studies are comparable because they calculate/present bioavailable iron concentrations (in addition to total dissolved iron concentrations). Data are incorporated from Sunda & Huntsman 1995; Rodriguez et al 2016; Rodriguez & Ho 2018. Links here: https://www.sciencedirect.com/science/article/pii/030442039500035P; https://www.frontiersin.org/articles/10.3389/fmicb.2016.00082/full; https://www.frontiersin.org/articles/10.3389/fmicb.2018.00142/full

**fig_s3_allalgae_growthcomparison.Rmd** Rmarkdown file for figure S3. Visualizes microalgae specific growth by bioavialable iron concentration for different lineages. Calls upon the growth comparison excel file.
 
**all_posthoc_stats_output.csv** Bivariate kruskal-wallis output for metal content, uptake & efficiency. Pairwise comparisons between each treatment. Please see description of abbreviations in the general remarks (above) for proper interpretation of abbreviations in "comparisons" column.

## Abstract
Iron (Fe) is essential to the physiology and growth of marine phytoplankton. It remains
unclear how important iron is to the functional ecology of symbiotic dinoflagellates in
the family Symbiodiniaceae, and whether limitations in iron ultimately affect the health
and productivity of coral hosts, especially during of episodes of ocean warming. Five
Symbiodiniaceae species (spanning three genera) were used to investigate the effects
of reduced iron availability on cell growth and the acquisition of other trace metals.
When grown under iron replete conditions, intracellular iron quotas (content) reflected
a large biochemical demand and ranged from 7.8-23.1 mmol Fe mol P-1.
Symbiodinium necroappetens was the only species that acclimated and maintained
high growth rates while subjected to the lowest iron treatment (250 pM Fe´). Cultures
surviving under low iron concentrations experienced changes in cellular concentrations
(and presumably their use as co-factors) of other trace metals (e.g. zinc, copper,
cobalt, manganese, nickel, molybdenum, vanadium), in ways that were species
specific, and possibly related to the natural ecology of each species. These changes in
trace metal contents may have cascading effects on vital biochemical functions such
as metalloenzyme activities, photosynthetic performance, and macronutrient
assimilation. Furthermore, these species-specific responses to iron limitation provides
a basis for investigations on how iron availability effects cellular processes among
species and genera of Symbiodiniaceae, and ultimately how metal shortages of
modulates the response of coral-algal mutualisms to physiological stressors.

### Feel free share this paper/github on twitter (@HannahGReich) if you agree that Symbiodiniaceae trace metal needs are pretty neat :-)


