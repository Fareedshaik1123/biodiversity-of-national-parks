Project Overview
This project analyzes biodiversity observations across U.S. national parks using two datasets: observations.csv and species_info.csv. The goal is to explore species diversity, conservation statuses, and observation patterns across four national parks: Great Smoky Mountains, Yosemite, Bryce, and Yellowstone. The analysis includes data exploration, visualization, and insights into species categories and their conservation needs.

Methodology
Data Preprocessing
Loading Datasets: The species_info.csv dataset contains species details (category, scientific name, common names, conservation status), while observations.csv includes observation counts across parks.
Handling Missing Data: Missing conservation statuses in species_info.csv were filled with "Doing well" to indicate no immediate concern.
Merging Data: The datasets were explored individually, with potential for merging on scientific_name for deeper analysis (not fully implemented in the notebook).
Feature Engineering
Species Categorization: Species were grouped by category (e.g., Mammal, Bird, Vascular Plant) and conservation_status (e.g., Endangered, Species of Concern).
Park Analysis: Observation data was aggregated by park_name to assess biodiversity distribution.
Visualization
A bar plot was created using seaborn to visualize observations of bats per week across parks, though the obs_by_park DataFrame and Protected_Species variable were not fully defined in the provided code snippet.
Results
Species Diversity: The dataset includes 5,541 unique species across 7 categories, with Vascular Plants (4,470) being the most represented and Reptiles (79) the least.
Conservation Status:
Endangered: 16 species
In Recovery: 4 species
Species of Concern: 161 species
Threatened: 10 species
Doing well: 5,633 species (after filling NaN values)
Observation Coverage: A total of 23,296 observations were recorded across four national parks, with each park showing distinct biodiversity patterns (visualized in the bar plot).
Conclusion
This project successfully explored biodiversity and conservation statuses across U.S. national parks. The analysis highlights the prevalence of Vascular Plants and identifies species under various levels of conservation concern. The visualization of bat observations (pending complete code) suggests park-specific ecological insights, demonstrating the potential for data-driven conservation strategies.

Future Work
Complete Visualization: Define obs_by_park and Protected_Species to fully implement the bat observation bar plot and extend to other species.
Statistical Analysis: Conduct hypothesis testing (e.g., chi-square tests) to assess relationships between conservation status and species categories.
Time-Series Analysis: If temporal data is available, analyze observation trends over time.
Interactive Dashboard: Develop a tool for park managers to monitor species observations and conservation priorities in real-time.
Acknowledgements
Data Source: The datasets (observations.csv and species_info.csv) were provided as part of the project (source not specified; assumed from an educational or open data repository).
Open Source Libraries:
pandas for data manipulation
numpy for numerical operations
matplotlib and seaborn for visualization
Jupyter Notebook for interactive analysis