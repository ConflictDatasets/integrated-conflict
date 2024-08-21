# integrated-conflict

This repository contains code and documentation related to the Ethiopia integrated conflict dataset between January 1997 and December 2017.

The main code document contains details on downloading existing conflict datasets from their respective websites. The final merged conflict dataset is available on [OSF](https://osf.io/6vkm8/), as are the individual taxonomy datasets. The final merged conflict dataset should be cited as: Andriano, Liliana, Mathis Ebbinghaus, and Thomas James Brailey. 2023. “Building a comprehensive database on conflict: Ethiopia, 1997–2017.” OSF. https://doi.org/10.17605/osf.io/6vkm8

To reproduce the final dataset, one needs the following files:

1. event_tax.csv
1. prec_tax.csv
1. actor_tax.csv
1. 1997-01-01-2022-01-31-Ethiopia.csv
1. globalterrorismdb_0221dist.csv
1. ged201.RData
1. SCAD2018Africa_Final.csv

We provide the first three dataset, but we provide written instructions for downloading the other four datasets, this is because datasets such as ACLED, though publicly available, require researchers to create an account and provide private security keys in order to download their data. Below we describe the procedure to download each of the four datasets. 

## Downloading ACLED

1. Go to https://acleddata.com/data-export-tool/.
1. Create an account.
1. Under the `Data Export Tool` heading, paste your access key, specify `From` to be "01/01/1997" and `To` to be "31/01/2022". `Event Type`, `Sub Event Type`, `Actor Type`, `Actor`, `Region`, and `Location` should take the value of `All`. `Country` should be `Ethiopia` and `Keyword` should be left blank. Lastly, provide the email address associated with your account, and set `Export Type` to be `Actor Based`. 
1. Hit `Export`. 
1. Save data in a folder within your project called `ACLED`.

## Downloading GTD

1. Go to https://www.start.umd.edu/gtd/contact/download
1. Provide contact and institutional details. `Country` should be set to `Ethiopia` (you will be given all years in the GTD dataset, but you will subset these values in the code chunk below).
1. Once you have received approval, download the data and store it in a folder called "GTD".

## Downloading GED

1. Go to https://ucdp.uu.se/downloads/. 
1. Scroll down to `UCDP Georeferenced Event Dataset (GED) Global version`.
1. Click on the `R` tab.
1. Save the data in a folder called `UCDP GED/ged201-RData`.

## Downloading SCAD

1. Go to https://www.strausscenter.org/ccaps-research-areas/social-conflict/database/. 
1. Click on `Download SCAD—Africa`. 
1. Save the dataset in a folder called `UCDP GED`.

# Acknowledgement
This work was generously supported by the British Academy (BA/Leverhulme SRG21\210356) and the John Fell Oxford University Press (OUP) Research Fund.

