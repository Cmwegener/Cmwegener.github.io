# Welcome to my thesis

**Thesis overview:** My thesis focuses on the _Fucus distichus_ in San Francisco Estuary, looking at both its current status and how climate change could affect it in the future. To accomplish this there were two parts to my thesis: field work and an experiment. The field work took place at four field sites in Central San Francisco Bay with monthly surveys from June 2018 to Septemeber 2019. Population data was recorded in the field and samples were taken to be processed in the lab. The mesocosm experiment manipulated carbonate chemistry and salinity levels to study its affect on the reproductive output (oogonia) of _Fucus distichus_.

### **Research Questions**
1. What is the distribution and abundance of _F. distichus_ in SFE and how does the population structure change over time? 
2. What is the reproductive phenology of _F. distichus_ in SFE? 
3. Is variation in salinity, air temperature, or pH associated with changes in abundances or reproductive effort of _F. distichus_ populations in SFE? 
4. Do changes to estuarine salinity and pH influence the reproductive output of _F. distichus_?

### **Data and calculations**  
**Data:** Both raw and calculated data available [here](https://github.com/Cmwegener/thesis/tree/master/data) 
**Field data calculations:** [markdown with calculations]((https://cmwegener.github.io/thesis/calculations.html)  
**Environmental data wrangling:** [data wrangling and final dataset](https://cmwegener.github.io/thesis/environmental_data.html), some of the raw data sets I downloaded are too large to upload on GitHub so I [removed unneeded columns](https://cmwegener.github.io/thesis/smaller_data_sets.html), [air](https://cmwegener.github.io/thesis/air.html)  
**Lining up environmental data with field data:** [data set-up](https://cmwegener.github.io/thesis/envir.field.html)  


### **1. What is the distribution and abundance of _F. distichus_ in SFE and how does the population structure change over time?** 
   - **Field site and bouy locations** [map](https://cmwegener.github.io/thesis/map_sites.pdf): We conducted monthly ecological *F. distichus* surveys at four sites from June 2018 to September 2019. Surveys were conducted at low tide once a month and at least three weeks apart between months. When we first surveying potential field sites, we referenced iNaturalist to see where *F. distichus* has been found. We picked four accessible representative sites to capture the variability of Central San Francisco Estuary (SFE). Field sites were located in Central SFE along the salinity gradient at Horseshoe Bay (37.83, -122.48), Brickyard Park (37.88, -122.50), Point Chauncy (37.89, -122.45), and Paradise Cay (37.92, -122.48). Each site has a monitoring buoy relatively close to each one so that we could characterize the salinity and temperature of each site. 
   - **Distribution of *Fucus distichus* in San Francisco Bay** [map](https://cmwegener.github.io/thesis/map_pic.html), [Rmarkdown](https://cmwegener.github.io/thesis/interactive_map.html): Distribution of *F. distichus* in San Francisco Estuary was determined by downloading 299 observations of *Fucus distichus* from iNaturalist (May 15, 2020). iNaturalist is a citizen science platform where users upload pictures of species with linked GPS coordinated. Only research grade observations of F. distichus in SFE on iNaturalist where downloaded. I then assessed each photo and assigned it as “attached,” “wrack,” or “unclear.” I then mapped this database in a map on R (package “leaflet”). [inat only](https://cmwegener.github.io/thesis/inat_only.html), [Josselyn West, 1985 only](https://cmwegener.github.io/thesis/jw_only.html)
  - **Phenology analysis** [mixed models, field data only](https://cmwegener.github.io/thesis/mixed_models_field.html)
  - **Percent cover** [Rmarkdown](https://cmwegener.github.io/thesis/percentcover.html): Standard quadrat transect sampling was used. Parallel to the shore, we placed a 15m transect through the middle of a healthy *F. distichus* population. The transect location was consistently within 0.5m throughout the sampling period. Random points (n=10) were selected along the transect and a 0.25m^2 quadrat was used for sampling. We measured percent cover in each quadrat.
  - **Total, large thalli and small thaiil density** [Rmarkdown](https://cmwegener.github.io/thesis/all_density.html): Density was measured by counting the number of holdfasts in the quadrat. Individuals with holdfasts outside of the quadrat were not counted. Individuals were then assigned into one of two size classes: small with individuals less than 12cm in length and large individuals longer than 12cm in length. 
  - **Opportunistic comparasion of 2018 versus 2019**  
      - **2018 vs 2019 *Fucus distichus* bed length** [table](https://cmwegener.github.io/thesis/length_table_pic.html), [Rmarkdown](https://cmwegener.github.io/thesis/length_table.html): This was an opportunist comparison of *F. distichus* in May 2018 versus May 2019. In May 2018, I scouted Central SFE for potential field sites of *F. distichus* looking for dense beds of at least 10 m in length. When I found dense beds, I recorded the GPS end points of the beds and in May 2019 I revisited the same sites. I used the “measure” tool on ArcGIS online to convert GPS points into lengths along the shoreline.

### **2. What is the reproductive phenology of _F. distichus_ in SFE?**
  - **Field Methods:** In the field, one specimen was randomly selected from each quadrat (n=10) for lab analysis. Samples were collected and immediately placed in sealed bags that were taken to the lab within 2 hours of collection times. Samples that were not immediately processed were placed in a dark refrigerator at a constant temperature (type, temp). Samples were processed within two weeks of collection. All samples were first inspected for and removed of epiphytes and invertebrates before proceeding. 
  - **Reproducitve anatomy and lab methods:** Reproductive tissue allocation was assessed in two ways. First, reproductive tissue allocation was calculated as a percentage of reproductive apices [diagram](https://cmwegener.github.io/thesis/repro_anatomy.pdf) (Graiff et al. 2017). Apices were considered reproductive with the presence of visible conceptacles. Second, reproductive tissue allocation was calculated by biomass. Reproductive apices were cut and separated from the vegetative portion of each sample. Samples were then placed in a drying oven at 17C for at least 48 hours (oven model). Dry reproductive and dry vegetative weights were then recorded to the nearest thousand decimal place on an analytical scale. We combined the density data and reproductive potential data to estimate oogonia/ow we calculated oogonia/0.25m^2 – calculated to incorporate oogonia per conceptacle, m^2 each month at each site. (conceptacle per reproductive apex, reproductive apex per adult thalli, and adult thalli per 0.25m^2 and was then square root transformed. this takes the oogonia in an individual thalli and scales it to an ecological context). These methods are based from Graiff (2017) and Pearson and Brawley (1996). I quantified reproductive potential of 3 of the 10 collected samples. These 3 samples were randomly selected. Reproductive potential is defined here as the number of oogonia within conceptacles of F. distichus. Quantifying the reproductive potential indicated how many eggs are available for release. From the 3 selected samples, I randomly selected a reproductive apex from each sample and I counted the number of conceptacles present. Then from each selected apex, I cut three conceptacles out to section with a razor blade, hydrate with water, and place it on a slide. Each slide was inspected under xmag/microscope where I counted the oogonia for each of the selected conceptacles [diagram](https://cmwegener.github.io/thesis/repro_anatomy.pdf).
  - **Varifying lab methods:** total dry weight vs total wet weight- [graph](https://cmwegener.github.io/thesis/dwt_vs_wwt.png), [Rmarkdown](https://cmwegener.github.io/thesis/dwt_vs_wwt.html)  
  - **Oogonia per meter:** [Rmarkdown](https://cmwegener.github.io/thesis/oogonia_per_meter.html)  
  - **Oogonia per thalli:** [Rmarkdown](https://cmwegener.github.io/thesis/oogonia_per_thalli.html) 
  - **Oogonia per conceptacle:** [Rmarkdown](https://cmwegener.github.io/thesis/oogonia_per_conceptacle.html)  
  - **Percent Reproductive Apices:** [Rmarkdown](https://cmwegener.github.io/thesis/percent_ra.html)  
  - **Percent Reproductive Dry Weight:** [Rmarkdown](https://cmwegener.github.io/thesis/percent_repro_dryweight.html)  
  - **Reproductive percent cover in field:**[Rmarkdown](https://cmwegener.github.io/thesis/repro_state.html)  
  - **Reproductive dry weight vs reproductive apices:** [Rmarkdown](https://cmwegener.github.io/thesis/drw_vs_ra.html)
  - **Percent reproductive dry weight per thalli:** [Rmarkdown](https://cmwegener.github.io/thesis/percent_dwr.html)

### **3. Is variation in salinity, air temperature, or pH associated with changes in abundances or reproductive effort of _F. distichus_ populations in SFE?** 
**Environmental data** [graphs](https://cmwegener.github.io/thesis/envi_graphs.html)
    - [pH vs dissolved oxygen](https://cmwegener.github.io/thesis/ph.v.do.html)

### 4. Do changes to estuarine salinity and pH influence the reproductive output of _F. distichus_?
**Mesocosm Experiment: Efects of pH and salinity on oogonia released**
**Experimental set up and design**
  - Mesocosm design: [diagram](https://cmwegener.github.io/thesis/exp_set_up.pdf)
  - In-unit seaweed platforms: [diagram](https://cmwegener.github.io/thesis/seaweed_platforms.pdf)

**Oogonia released under different pH and salinity conditions**
  - Calculations: [Rmarkdown](https://cmwegener.github.io/thesis/meso_calc.html)
  - Heatmap: [Rmarkdown](https://cmwegener.github.io/thesis/heatmap.html)
  - Interactive effect of salinity and pH on oogonia release: [graph with markers](https://cmwegener.github.io/thesis/sal_ph_oo_3d_pic.html), [graph with surface contour](https://cmwegener.github.io/thesis/sal_ph_oo_surface_pic.html), [Rmarkdown](https://cmwegener.github.io/thesis/sal_ph_oo.html), [potential picture for print](https://cmwegener.github.io/thesis/sal_ph_oo.jpeg)
  - Effect of temperature, dissolved oxygen, ph, and salinity on oogonia release: [graph](https://cmwegener.github.io/thesis/temp_do_sal_ph_oo.png), [Rmarkdown](https://cmwegener.github.io/thesis/temp_do_sal_ph_oog.html)
  
**Unit conditions**
  - Unit conditions: [graph](https://cmwegener.github.io/thesis/all_unit_conditions.png), [Rmarkdown](https://cmwegener.github.io/thesis/all_unit_conditions.png)
  - Salinity Hach readings: [graph](https://cmwegener.github.io/thesis/salinity_hach.png), [Rmarkdown](https://cmwegener.github.io/thesis/salinity_hach.html)
  - pH Hach readings: [graph](https://cmwegener.github.io/thesis/ph_hach.png), [Rmarkdown](https://cmwegener.github.io/thesis/ph_hach.html)
  - Temperature Hach readings: [graph](https://cmwegener.github.io/thesis/temp_hach.png), [Rmarkdown](https://cmwegener.github.io/thesis/temp_hach.html)
  - Dissolved Oxygen Hach readings: [graph](https://cmwegener.github.io/thesis/do_hach.png), [Rmarkdown](https://cmwegener.github.io/thesis/do_hach.html)

**Experimental thalli**
  - Thalli weight: [graph](https://cmwegener.github.io/thesis/thalli_weight.png), [Rmarkdown](https://cmwegener.github.io/thesis/thalli_weight.html)
  - PAR: [graph](https://cmwegener.github.io/thesis/par.png), [Rmarkdown](https://cmwegener.github.io/thesis/par.html)
  - Percent reproductive dry weight per thalli: [graph](https://cmwegener.github.io/thesis/exp_percent_dwr.png), [Rmarkdown](https://cmwegener.github.io/thesis/exp_percent_dwr.html)
  - Percent Reproductive Apices: [graph](https://cmwegener.github.io/thesis/exp_percent_ra.png), [Rmarkdown](https://cmwegener.github.io/thesis/exp_percent_ra.html)
 
 **Verifying Hach readings**
   - Hach vs discrete pH: [graph](https://cmwegener.github.io/thesis/hach_vs_discrete.png), [Rmarkdown](https://cmwegener.github.io/thesis/hach_vs_discrete.html)

### Discussion
  - Comparative reproductive phenology table: [table](https://cmwegener.github.io/thesis/phenology_table_pic.html), [Rmarkdown](https://cmwegener.github.io/thesis/phenology_table.html)




**Old attempts and approaches no longer being used (double check before removing)
  - Enviormental data [all](https://cmwegener.github.io/thesis/envi_graphs.html), [salinity](https://cmwegener.github.io/thesis/salinity.html), [pH](https://cmwegener.github.io/thesis/ph.html), [dissolved oxygen](https://cmwegener.github.io/thesis/dissolved.oxygen.html), [water temeperature](https://cmwegener.github.io/thesis/water.temp.html), [metadata](https://cmwegener.github.io/thesis/envi.metadata.html)
  - [data set-up](https://cmwegener.github.io/thesis/set-up.html)
  - [data question](https://cmwegener.github.io/thesis/eos_data_check.html), [revised](https://cmwegener.github.io/thesis/eos_new.html)
  - [analysis attempt](https://cmwegener.github.io/thesis/analysis.html), [finding best fit](https://cmwegener.github.io/thesis/model_fuc_density.html), [new](https://cmwegener.github.io/thesis/analysis_attempt.html), 

