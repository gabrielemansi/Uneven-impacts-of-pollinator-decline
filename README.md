# Pollinator decline reveals uneven impacts of climate-driven biodiversity loss — Datasets

This record provides the data underlying the working paper "Pollinator decline reveals uneven impacts of climate-driven biodiversity loss", a climate-driven, multi-model assessment of the macroeconomic consequences of pollinator decline in the European Union. Projected changes in wild-pollinator distribution are translated into crop-yield losses and then into regional economic impacts with a sub-national computable general equilibrium (CGE) model. The record is organised in three folders, one for each stage of the modelling chain.

## Citation

> Campoleoni Mansi, G. A., Standardi, G., & Bosello, F. (2026). *Pollinator decline reveals uneven impacts of climate-driven biodiversity loss* [Datasets]. Zenodo. https://doi.org/10.5281/zenodo.20542846


## Authors

| Author | Affiliations |
|---|---|
| G. A. Campoleoni Mansi | 1, 2, 3 |
| G. Standardi | 1, 4 |
| F. Bosello | 1, 2, 3 |

1. CMCC Foundation – Euro-Mediterranean Center on Climate Change, Via Marco Biagi 5, 73100 Lecce, Italy
2. RFF-CMCC European Institute on Economics and the Environment, Via Bergognone 34, 20144 Milan, Italy
3. Ca' Foscari University of Venice, Dorsoduro 3246, 30123 Venice, Italy
4. Department of Environmental Science and Policy, University of Milan, Via Celoria 2, 20133 Milan, Italy

**Contact:** G. A. Campoleoni Mansi, CMCC Foundation — [gabriele.mansi@cmcc.it](mailto:gabriele.mansi@cmcc.it)

## Study summary

The study delivers the first climate-driven, multi-model assessment of the macroeconomic consequences of pollinator decline at sub-national resolution for the EU. It links wild-pollinator distribution projections to 129 crops to quantify how biodiversity loss propagates through agricultural systems across 122 EU regions.
An integrated modelling chain links an ensemble of pollinator species distribution projections to a sub-national CGE model for the EU. Changes in pollination services propagate through the agricultural sector into the wider economy, resolved across 129 crops and 122 EU administrative units.

| Stage | Folder | Content | Spatial units | Years |
|---|---|---|---|---|
| 1 | `pollination_potential_scenarios/` | Cumulative change in pollination potential relative to 2020 | EU-27, Member States, 122 CGE regions | 2030, 2050, 2070 |
| 2 | `land_productivity_loss/` | Change in crop yields due to projected changes in pollination services, by crop and by CGE crop sector | NUTS 0–3 regions | 2020–2080, 5-year steps |
| 3 | `macroeconomic_output/` | CGE results: regional GDP and value of output of the agricultural sector and of each crop sector | 122 CGE regions, EU-27, rest of the world | 2017, 2020–2070, 5-year steps |


## Scenarios

All three stages cover the same 18 scenarios, drawn from three families of pollinator projections: PREST, IIASA and GHSB. Scenarios combine a Shared Socioeconomic Pathway (SSP) with a Representative Concentration Pathway (RCP); `CLIM` scenarios are identified by the RCP only.

| Scenario | SSP | RCP | Stage 2 folder | Stage 2 column prefix | Stage 3 sheet |
|---|---|---|---|---|---|
| PREST-CLIM 2.6 | – | 2.6 | `Prestele_CLIM` | `RCP2_6` | `PREST_CLIM_2.6` |
| PREST-CLIM 4.5 | – | 4.5 | `Prestele_CLIM` | `RCP4_5` | `PREST_CLIM_4.5` |
| PREST-CLIM 8.5 | – | 8.5 | `Prestele_CLIM` | `RCP8_5` | `PREST_CLIM_8.5` |
| PREST-1 2.6 | SSP1 | 2.6 | `Prestele_SSPs` | `SSP1_2_6` | `PREST_1_2.6` |
| PREST-1 4.5 | SSP1 | 4.5 | `Prestele_SSPs` | `SSP1_4_5` | `PREST_1_4.5` |
| PREST-3 4.5 | SSP3 | 4.5 | `Prestele_SSPs` | `SSP3_4_5` | `PREST_3_4.5` |
| PREST-3 8.5 | SSP3 | 8.5 | `Prestele_SSPs` | `SSP3_8_5` | `PREST_3_8.5` |
| PREST-5 8.5 | SSP5 | 8.5 | `Prestele_SSPs` | `SSP5_8_5` | `PREST_5_8.5` |
| IIASA-CLIM 2.6 | – | 2.6 | `IIASA_CLIM` | `RCP2_6` | `IIASA_CLIM_2.6` |
| IIASA-CLIM 4.5 | – | 4.5 | `IIASA_CLIM` | `RCP4_5` | `IIASA_CLIM_4.5` |
| IIASA-CLIM 7.0 | – | 7.0 | `IIASA_CLIM` | `RCP7_0` | `IIASA_CLIM_7.0` |
| IIASA-CLIM 8.5 | – | 8.5 | `IIASA_CLIM` | `RCP8_5` | `IIASA_CLIM_8.5` |
| IIASA-2 2.6 | SSP2 | 2.6 | `IIASA_SSPs` | `RCP_2_6` | `IIASA_2_2.6` |
| IIASA-2 4.5 | SSP2 | 4.5 | `IIASA_SSPs` | `RCP_4_5` | `IIASA_2_4.5` |
| IIASA-2 7.0 | SSP2 | 7.0 | `IIASA_SSPs` | `RCP_7_0` | `IIASA_2_7.0` |
| GHSB-1 2.6 | SSP1 | 2.6 | `GHSB_SSPs` | `RCP2_6` | `GHSB_1_2.6` |
| GHSB-3 6.0 | SSP3 | 6.0 | `GHSB_SSPs` | `RCP6_0` | `GHSB_3_6.0` |
| GHSB-5 8.5 | SSP5 | 8.5 | `GHSB_SSPs` | `RCP8_5` | `GHSB_5_8.5` |

- **Scenario** is the label used in stage 1. The `all_shocks` tables of stage 2 use the same labels, with an underscore in the CLIM scenarios (e.g. `PREST_CLIM 2.6`, `IIASA_CLIM 4.5`).
- **Stage 2 folder** is shortened: full folder names end in `_INCA_cum_2020_2080` (crop level) or `_INCA_cum_2020_2080pct_wrt_2020` (sector level).
- **Stage 2 column prefix** identifies the scenario within its family folder; value columns are named `<prefix>_<year>` (e.g. `SSP3_8_5_2050`).

## Folder structure

```text
pollination_potential_scenarios/
└── pollination_scenarios_wrt_2020.{xlsx,rds}

land_productivity_loss/
├── all_crops_productivity_shocks/
│   └── <family>_INCA_cum_2020_2080/                  5 folders, one per scenario family
│       └── <crop>/                                   103 folders, one per crop
│           └── shock_<family>_INCA_cum_2020_2080_<crop>.{csv,xlsx,rds}
└── agri_sectors_productivity_shocks/
    ├── scenarios/
    │   └── <family>_INCA_cum_2020_2080pct_wrt_2020/  5 folders, one per scenario family
    │       └── pct_wrt_2020_<sector>.{xlsx,rds}      6 files: Agri_sector, c_b, gro, ocr, osd, v_f
    ├── all_shocks/
    │   ├── all_shocks_wrt_2020.{xlsx,rds}
    │   ├── all_shocks_wrt_2020_NUTS.{xlsx,rds}
    │   └── all_shocks_wrt_2020_NUTS_long.{xlsx,rds}
    └── sensitivity_analysis/
        ├── all_shocks_2050_sensitivity_EU27.{xlsx,rds}
        ├── all_shocks_2050_sensitivity_NUTS.{xlsx,rds}
        ├── all_shocks_2070_sensitivity_EU27.{xlsx,rds}
        └── all_shocks_2070_sensitivity_NUTS.{xlsx,rds}

macroeconomic_output/
└── Pollination_impact_all_results.{xlsx,rds}
```

`<family>` is one of `GHSB_SSPs`, `IIASA_CLIM`, `IIASA_SSPs`, `Prestele_CLIM`, `Prestele_SSPs`.

## 1. Pollination potential scenarios

**Folder:** `pollination_potential_scenarios/` · **File:** `pollination_scenarios_wrt_2020` (.xlsx, .rds)

Future pollination potential is computed at 1 km × 1 km resolution for the 18 scenarios. For each scenario and five-year step, the per-period changes are cumulated pixel by pixel and applied multiplicatively to the 2020 baseline. The file reports the resulting cumulative percentage change in habitat suitability relative to 2020, aggregated to the EU-27, the 27 Member States and the 122 regions of the CGE model, for 2030, 2050 and 2070. Negative values indicate a decline.

| Column | Description |
|---|---|
| `scenario` | Scenario label (see Scenarios) |
| `NUTS_ID` | Country code (Member States; `EU` for the EU-27) or NUTS code of the CGE region |
| `LEVL_CODE` | NUTS level of `NUTS_ID` (0, 1 or 2) |
| `CNTR_NAME` | Country name, or name of the CGE region (e.g. `EastAustria`, `bgr`) |
| `2030`, `2050`, `2070` | Cumulative change relative to 2020 (%) |

Each scenario has 150 rows: 28 for the Member States and the EU-27, followed by the 122 CGE regions. Member States modelled as a single CGE region therefore appear twice (e.g. `BG` as `Bulgaria` and as `bgr`). CGE regions are NUTS 0, 1 or 2 regions identified by pre-2024 NUTS codes; this table also provides the correspondence between the CGE region names used in stage 3 and NUTS codes.

Example (`PREST-CLIM 4.5`):

| scenario | NUTS_ID | LEVL_CODE | CNTR_NAME | 2030 | 2050 | 2070 |
|---|---|---:|---|---:|---:|---:|
| PREST-CLIM 4.5 | EU | 0 | EU | -13.11 | -29.06 | -31.86 |
| PREST-CLIM 4.5 | AT1 | 1 | EastAustria | -13.74 | -31.43 | -35.10 |
| PREST-CLIM 4.5 | BG | 0 | bgr | -14.39 | -30.98 | -33.01 |
| PREST-CLIM 4.5 | ES11 | 2 | Galicia | -12.35 | -25.10 | -26.08 |

## 2. Land productivity loss

**Folder:** `land_productivity_loss/`

Projected pollination shocks on crop yields, i.e. changes in crop yields due to projected changes in pollination services. All values are percentage changes in crop yield relative to 2020: values for 2020 are 0 and negative values are yield losses on 2020 cropland area. The data support analysis of climate change impacts on crop yields through pollination services at European regional (NUTS) level.

Tables cover 1,728 NUTS 2024 regions at levels 0 to 3 in 39 European countries: the EU-27 plus AL, BA, CH, IS, LI, ME, MK, NO, RS, TR, UA and XK. The `all_shocks` tables are restricted to the 1,502 regions of the EU-27. The Canary Islands, the Azores, Madeira and the French outermost regions are not included.

### 2.1 Crop-level shocks — `all_crops_productivity_shocks/`

One file per scenario family and crop (5 × 103 files), each provided as .csv, .xlsx and .rds, with one row per region.

| Column | Description |
|---|---|
| `NUTS_ID` | NUTS 2024 region code (e.g. `AT127`) |
| `LEVL_CODE` | NUTS level (0 = country, 1, 2, 3) |
| `CNTR_CODE` | Two-letter country code, Eurostat convention (e.g. `AT`, `EL`) |
| `NAME_LATN` | Region name in Latin script |
| `nuts_total_hectares` | Area of the crop in the region (ha), used as aggregation weight |
| `base_name_crop` | Crop name |
| `<prefix>_<year>` | Yield change relative to 2020 (%) for the scenario identified by `<prefix>` (see Scenarios), 2020–2080 in 5-year steps |

Example (`IIASA_CLIM`, plum):

| NUTS_ID | LEVL_CODE | CNTR_CODE | NAME_LATN | nuts_total_hectares | base_name_crop | RCP2_6_2020 | RCP2_6_2025 | RCP2_6_2030 | … |
|---|---:|---|---|---:|---|---:|---:|---:|---|
| AT127 | 3 | AT | Wiener Umland/Südteil | 279.88 | plum | 0 | -2.46 | -5.81 | … |
| AT130 | 3 | AT | Wien | 40.13 | plum | 0 | -0.66 | -1.57 | … |
| AT211 | 3 | AT | Klagenfurt-Villach | 74.53 | plum | 0 | -0.90 | -2.62 | … |
| AT212 | 3 | AT | Oberkärnten | 132.89 | plum | 0 | -0.05 | -0.12 | … |

**Crops (103):** alfalfa, almond, aniseetc, apple, apricot, artichoke, asparagus, avocado, banana, bean, beetfor, berrynes, blueberry, broadbean, buckwheat, cabbage, cabbagefor, carob, castor, cauliflower, cherry, chestnut, chickpea, chicory, chilleetc, citrusnes, cotton, cowpea, cranberry, cucumberetc, currant, date, eggplant, fig, flax, fornes, fruitnes, gooseberry, grape, grapefruitetc, greenbean, greenbroadbean, greencorn, greenonion, groundnut, kiwi, legumenes, lemonlime, lettuce, linseed, maize, maizefor, melonetc, melonseed, mixedgrain, mixedgrass, mustard, nutnes, oilseedfor, oilseednes, okra, olive, onion, orange, peachetc, pear, peppermint, persimmon, pimento, pineapple, plum, poppy, potato, pulsenes, pumpkinetc, quince, rapeseed, rasberry, safflower, sesame, sisal, sourcherry, soybean, spinach, stonefruitnes, strawberry, stringbean, sugarbeet, sugarcane, sunflower, swedefor, sweetpotato, tangetc, taro, tea, tobacco, tomato, tropicalnes, turnipfor, vegetablenes, vegfor, watermelon, yam.

In crop names, `nes` stands for "not elsewhere specified", `etc` groups related crops and `for` denotes forage crops.

### 2.2 Sector-level shocks — `agri_sectors_productivity_shocks/`

Crop-level shocks aggregated to the five crop sectors of the CGE model:

| Code | Crop sector |
|---|---|
| `v_f` | Vegetables, fruits and nuts |
| `osd` | Oilseeds |
| `gro` | Cereals, wheat and rice |
| `c_b` | Sugar cane and sugar beet |
| `ocr` | Other crops and fibres |
| `Agri_sector` | Aggregate of the five crop sectors |

**`scenarios/`** — one folder per scenario family and one file per sector, with the same layout as the crop-level files (`NUTS_ID`, `LEVL_CODE`, `CNTR_CODE`, `NAME_LATN`, `<prefix>_<year>` for 2020–2080). The column `total_area` (ha) replaces `nuts_total_hectares` and `base_name_crop`: it is the crop area of the sector in the region and the weight used for aggregation. `Agri_sector` is the `total_area`-weighted mean of the five sectors.

**`all_shocks/`** — the 18 scenarios in a single table, for the EU-27 and the years 2030, 2050 and 2070.

| File | Regions | Layout |
|---|---|---|
| `all_shocks_wrt_2020` | 27 Member States | Wide: one row per sector, region and year; one column per scenario |
| `all_shocks_wrt_2020_NUTS` | 1,502 EU NUTS 0–3 regions | Wide, as above |
| `all_shocks_wrt_2020_NUTS_long` | 1,502 EU NUTS 0–3 regions | Long: one row per sector, region and scenario; one column per year |

Columns: `crop_sector` (sector code), `NUTS_ID`, `LEVL_CODE`, `CNTR_NAME` (country name), `year` (wide files) or `scenario` (long file), followed by the values (%).

**`sensitivity_analysis/`** — spread of the sector shocks across the 18 scenarios, in 2050 and 2070.

| File | Regions |
|---|---|
| `all_shocks_<year>_sensitivity_EU27` | 27 Member States and the EU-27 (`EU`) |
| `all_shocks_<year>_sensitivity_NUTS` | 1,728 NUTS 0–3 regions |

Columns: `crop` (sector name), `NUTS_ID`, `LEVL_CODE`, `NAME_LATN`, `total_area` (EU27 files only), and `MAX`, `MED`, `MIN`, the maximum, median and minimum yield change across the 18 scenarios (%). As changes are mostly negative, `MIN` is the largest loss.

## 3. Macroeconomic output

**Folder:** `macroeconomic_output/` · **File:** `Pollination_impact_all_results` (.xlsx, .rds)

Results of the CGE model: changes in regional GDP, in the value of output of the aggregated agricultural sector, and in that of each crop sector considered by the model (vegetables, fruits and nuts; oilseeds; cereals, wheat and rice; sugar cane and sugar beet; other crops and fibres).

| Sheet | Content | Unit |
|---|---|---|
| `2017_GDP_VOM` | Base year 2017: GDP, population and value of output (VOM) by sector and region | Million US$; million inhabitants |
| `SSP1`, `SSP2`, `SSP3`, `SSP5` | Baseline projections without pollination shocks | Million US$ at 2017 prices |
| 18 scenario sheets (e.g. `PREST_CLIM_4.5`) | Projections with pollination shocks | Million US$ at 2017 prices |
| `Impacts_wrt_baseline` | Change of each variable relative to the baseline of the corresponding SSP | % |

Variables (column `variable`; `Variable % change w.r.t. baseline value` in `Impacts_wrt_baseline`):

| Variable | Description |
|---|---|
| `qgdp` | Real GDP |
| `qo_v_f`, `qo_osd`, `qo_gro`, `qo_c_b`, `qo_ocr` | Value of output of each crop sector (codes as in section 2.2) |
| `agri_sector` | Value of output of the aggregated agricultural sector (sum of the five crop sectors) |

Regions (column `NUTS`) are labelled `<number> <name>`: `1 RoW` is the rest of the world and `2` to `123` are the 122 EU regions of the model (e.g. `2 EastAustria`, `7 bgr`). `EU` is the sum of the 122 EU regions; in `2017_GDP_VOM`, `Total` is the sum of all regions. Region names are matched to NUTS codes in `pollination_scenarios_wrt_2020` (section 1). Level sheets report 2017 and 2020–2070 in 5-year steps; `Impacts_wrt_baseline` reports 2020–2070.

Example (`Impacts_wrt_baseline`, real GDP, values rounded to three decimals):

| Scenario | Variable | NUTS | 2030 | 2050 | 2070 |
|---|---|---|---:|---:|---:|
| PREST_CLIM_4.5 | qgdp | 2 EastAustria | -0.027 | -0.092 | -0.073 |
| PREST_CLIM_4.5 | qgdp | 73 Puglia | -0.048 | -0.196 | -0.319 |
| PREST_CLIM_4.5 | qgdp | 93 Norte | -0.046 | -0.110 | -0.185 |
| PREST_CLIM_4.5 | qgdp | EU | 0.019 | -0.084 | -0.079 |

## Conventions

- Changes are expressed in percent (e.g. `-2.46` = −2.46%); negative values indicate a decline.
- Stages 1 and 2 are expressed relative to 2020; stage 3 relative to the baseline without pollination shocks.
- Monetary values are in million US dollars at 2017 prices.
- Shocks are rounded to two decimals; sensitivity statistics to one decimal.
- Regions without crop area have zero shocks in the crop-level files and missing values in the sector-level files.
- Tables are provided as Excel (.xlsx) and R (.rds, readable with `readRDS()`) files; crop-level tables are also provided as CSV (UTF-8, comma-separated).

## Coverage notes

- The analysis focuses on the EU-27: shocks for non-EU countries are zero or close to zero.
- Malta shows no change in pollination potential or crop yields in any scenario; Cyprus shows no change in the PREST and GHSB scenarios.

## Source of pollinator projections.
> Gerber, G. (2026). *Dataset ACCREU D2.4: European pollinator species distribution models and pollination supply metrics under climate change* (Version 1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.22751031
> Ghisbain, G., Thiery, W., Massonnet, F. et al. (2024). Projected decline in European bumblebee populations in the twenty-first century. Nature 628, 337–341. https://doi.org/10.1038/s41586-023-06471-0 
> Prestele, R., Brown, C., Polce, C., Maes, J., & Whitehorn, P. (2021). Large variability in response to projected climate and land-use changes among European bumblebee species. Global Change Biology, 27(19), 4530--4545. https://doi.org/10.1111/gcb.15780

## Related data
> Campoleoni Mansi, G. A., Gerber, G., & Palazzo, A. (2026). *Pollination Shocks on European Crop Yields* (Version 1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23529106
Crop-level yield shocks under the IIASA-CLIM scenarios, produced within the ACCREU project.

## License

This dataset is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.

## Funding

This work was supported by the Assessing Climate Change Risk in Europe (ACCREU) project, funded by the European Commission under the Horizon Europe programme (grant agreement No. 101081358). Project website: [www.accreu.eu](https://www.accreu.eu/).

This dataset is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.

## Funding

This work was supported by the Assessing Climate Change Risk in Europe (ACCREU) project, funded by the European Commission under the Horizon Europe programme (grant agreement No. 101081358). Project website: [www.accreu.eu](https://www.accreu.eu/).
