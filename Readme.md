Jon Atkins
UC Berkely - CARB AHSC Project
August 19th, 2024

This directory contains all of the code associated with Task 2 and Task 4 modeling portion of the UC Berkeley project with CARB analyzing the AHSC program and its effect on VMT.

This analysis was conducted in July and August of 2024, and is organized as such.

# Structure

Within this folder is a lot of code, organized by a preceding number (indicating a group) and then a secondary number (indicating the order they should be run in). Within a group, the files are often dependent on previous files, however outside of a group, that is not necessarily the case

* 1: Data Load and modeling process (this was previously 5)

* 2: [archived] old modeling code (in Older Code)

* 3: [archived] other modeling attempts including the MARS

* 4: Mapping

* **models**: contains a folder for each iterative model, and the resulting visuals as well as a compilation of the notes from each iteration.

* **model_raw_outputs**: contains the raw coefficients, std. errors, etc. for each model iteration. The standard script saves this to a file in an "outputs" directory within the active directory.

* **checkin_visualizations**: contains a folder for each team check-in from July and August and the visualizations I presented at them.

* A note on RNotebooks: Most of my work is done in R notebooks (.Rmd files), which are best opened in Rstudio. They are then best run interactively and should prompt the user for anything that needs to be installed or included

  * I use the markdown format structure extensively to create a table of contents for each document, so I strongly recommend using the built-in `Outline` feature to navigate the code, it should make it much easier to follow
  
  * General coding principles: I will only use `<-` assignment and will start a new line with it so any blocks of code not beginning with `[variable_name] <- ` don't modify anything