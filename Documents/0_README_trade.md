---
editor_options:
  markdown:
    wrap: 72
output: pdf_document
---

# General Information

Data for Oceans Future analysis on hot spots for future conflict. Data
represents the percentage change in maximum catch potential by 2030
relative to present for two climate change scenarios.

# Method

Detailed information from the DBEM can be found in Cheung et al 2016.
The DBEM outputs have been transformed into percentage change in Maximum
Catch Potential, MCP, (a proxy of Maximum Sustainable Yield -MSY) by
2030 relative to the historical time period. For this analysis, the
historical period represents the average of 1995 to 2015 to match the
ESM and catch observation data used while 2030 represents the average
results of 2020 to 2039. This was done to reduce the system's natural
variability.

For each ESM, species and EEZ in the hot-spot analysis, we first
aggregated the MCP in all 0.5 x 0.5 grid cells by year. Then we average
the EEZ yearly MCP by the two time periods to reduce climate
variability. Next, we compute the percentage change in MCP from the
historical period relative to the future (i.e., ((2030 -
historical)/abs(historical)) \* 100 ). Finally, we estimated the average
(i.e., `mean_mcp_delta_2030`), ± s.d (i.e., `sd_mcp_delta_2030`). of
the percentage change across the three ESMs.

Cheung, W. W. L., et al . 2016. Structural uncertainty in projecting
global fisheries catches under climate change. Ecol Model 325: 57–66.

# File Metadata

-   `taxon_key`, Species ID. See `dbem_spp_list.csv` for reference list.
    note that these match the Sea Around Us ID numbers
-   `eez_name`, Name of the EEZ according to the Sea Around Us
    classification. Note that only the EEZs in the hot spot analysis
    were included
-   `ssp`, Climate change scenarios (Shared Socioeconomic Pathways),
    1-2.6 (low emissions) and 5-8.5 (high emissions)
-   `mean_mcp_delta_2030`, Mean percentage change in Maximum Catch
    Potential by 2030 relative to the historical period (1995-2015)
    across the three ESMs
-   `sd_mcp_delta_2030`, Standard deviation of the percentage change in
    Maximum Catch Potential by 2030 relative to the historical period
    (1995-2015) across the three ESMs

# Runs Metadata

-   Runs by: Juliano Palacios
    ([j.palacios\@oceans.ubc.ca](mailto:j.palacios@oceans.ubc.ca){.email})
-   Version: DBEM_v2
-   CMIP: CMIP6
-   ESMs: GFDL, IPSL, MPIS
-   SSPs: 1-2.6 & 5-8.5
-   nspp: 936
-   FHS: 1.00 (Fishing level in the high seas)
-   FEEZ: 1.00 (Fishing level in the EEZs)
-   MPAs: no_mpa (Does not includes marine protected areas)
-   time-frame: 1995-2040
