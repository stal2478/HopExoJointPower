# HopExoJointPower
Participant data from "The spring stiffness profile within a passive, full-leg exoskeleton affects lower-limb joint mechanics while hopping". The manuscript is currently under peer-review in Journal of the Royal Society Interface.

# Software & Packages
R version 3.2.2 <br>
RStudio 2023.06.1

# Data
Marker and device data were collected via Vicon Nexus, and inverse dynamics calculations were performed in Visual 3D.
This dataset represents the participant-average data for each hopping condition, and has been parsed into files for time-series or discrete datasets.
All files are in long format. The R Markdown scripts will transform data into wide format for easier viewing, and descriptions of variables are provided within the markdown files.

- ang_data.csv - Peak joint flexion, extension, and range of motion throughout hop cycle.
- kin_data.csv - Whole body kinematic and kinetic data,
- mom_data.csv - Overall (Exo + MTU), exoskeleton, and muscle-tendon unit (MTU) contributions to average internal joint moments.
- pow_data.csvs - Overall (Exo + MTU), exoskeleton, and muscle-tendon unit (MTU) contributions to average internal joint powers.
- time_series.csv - Instantaneous joint angle, moment, and power (separated by contribution sources, joint, condition, and participant) .

# Scripts

- HEJP_stats.Rmd - R Markdown for calling each data file for one-way, repeated measures anovas and multiple comparisons testing.
- HEJP_plots.Rmd - R Markdown for creating plots seen in publication.
