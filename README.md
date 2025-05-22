# Cleaning the shorebird survey data 


## The data set

ARCTIC SHOREBIRD DEMOGRAPHICS NETWORK [https://doi.org/10.18739/A2222R68W](https://doi.org/10.18739/A2222R68W)

Data set hosted by the [NSF Arctic Data Center](https://arcticdata.io) data repository 

Field data on shorebird ecology and environmental conditions were collected from 1993-2014 at 16 field sites in Alaska, Canada, and Russia.

![Shorebird, copyright NYT](https://static01.nyt.com/images/2017/09/10/nyregion/10NATURE1/10NATURE1-superJumbo.jpg?quality=75&auto=webp)

Data were not collected every year at all sites. Studies of the population ecology of these birds included nest-monitoring to determine the timing of reproduction and reproductive success; live capture of birds to collect blood samples, feathers, and fecal samples for investigations of population structure and pathogens; banding of birds to determine annual survival rates; resighting of color-banded birds to determine space use and site fidelity; and use of light-sensitive geolocators to investigate migratory movements. 

Data on climatic conditions, prey abundance, and predators were also collected. Environmental data included weather stations that recorded daily climatic conditions, surveys of seasonal snowmelt, weekly sampling of terrestrial and aquatic invertebrates that are prey of shorebirds, live trapping of small mammals (alternate prey for shorebird predators), and daily counts of potential predators (jaegers, falcons, foxes). Detailed field methods for each year are available in the `ASDN_protocol_201X.pdf` files. All research was conducted under permits from relevant federal, state, and university authorities.

See `01_ASDN_Readme.txt` provided in the [course data repository](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-spring-2024-class-data) for full metadata information about this data set.

# DATA & FILE OVERVIEW

1. File List: 

## Repository Structure: 

```bash

├── data
│   ├── processed
│   │   ├── all_cover_fixed_JORGENSEN.csv
│   │   ├── snow_cover.csv
│   ├── raw
│   │   ├── 01_ASDN_Readme.txt
│   │   ├── ASDN_Daily_species.csv
│   │   ├── ASDN_Snow_survey.csv
├── docs
│   ├── data-cleaning_files/libs
│   │   ├── bootstrap
│   │   │   ├── bootstrap-icons.css
│   │   │   ├── bootstrap-icons.woff
│   │   │   ├── bootstrap.min.css
│   │   │   ├── bootstrap.min.js
│   │   ├── clipboard
│   │   │   ├── clipboard.min.js
│   │   ├── quarto-html
│   │   │   ├── anchor.min.js
│   │   │   ├── popper.min.js
│   │   │   ├── quarto-syntax-highlighting.css
│   │   │   ├── quarto.js
│   │   │   ├── tippy.css
│   │   │   ├── tippy.umd.min.js
│   └── data-cleaning.html
├── .Rprofile
├── .gitignore
├── README.md
├── all_cover_fixed_JORGENSEN.qmd
├── bren-meds213-data-cleaning.Rproj
└── data-cleaning_empty.qmd
```

Description: The data folder of this repository contains the arctic shorebirds data described above. The 'raw' folder contains the species presence and snow survey data, before it was cleaned in this analysis. The 'processed' folder contains the .csv files that are the result of the data cleaning which will be described in more detail below. 

The docs folder in this repository contains the folders and files that render the visuals for this assingment in a classroom setting. They are not relevant to the data cleaning described below. 

The all_cover_fixed_JORGENSEN.qmd file contains the described workflow and process behind the cleaning of this data. The data-cleaning_empty.qmd file is the file used for educational purposes to present the cleaning of the data. 


2. Relationship between files:

For the purposes of exploring the cleaning of the data, the 'raw' folder contains the unclean data, which was processed in the 'all_cover_fixed_JORGENSEN.qmd' file, and the output of this is stored in the 'processed' folder. 

3. Additional related data collected that was not included in the current data package:

Due to the ongoing updates of this data, it is the recommendation of the Arctic Shorebird Demographics Network that "Potential users of these data should first contact the relevant data author(s), listed below.  This will enable coordination in terms of updates/corrections to the data and ongoing analyses.  Key analyses of the data are in progress and will be included in the theses and dissertations of graduate students who collected these field data." These authors would be abreast with any current updates that may not currently be part of this dataset. These authors are: 

Barrow
	Rick Lanctot (richard_lanctot@fws.gov)
	Sarah Saalfeld (sarah_saalfeld@fws.gov)
	
Burntpoint
	Rod Brook (rod.brook@ontario.ca)
	Kim Bennet (Kim.Bennett@ontario.ca)
	Ken Abraham

Bylot Island
	Joël Bêty (joel_bety@uqar.ca)
	Jean-Francois Lamarre (jflamarre@gmail.com)

Cape Krusenstern
	Megan Boldenow (mboldenow@gmail.com)

Canning River
	Stephen Brown (sbrown@manomet.org)
	David Payer


Chaun, Ikpikpuk, Prudhoe
	Rebecca Bentzen (rbentzen@wcsc.org)
	Steve Zack
	Joe Liebezeit
	Martin Robards
	
Churchill
	Erica Nol (ericanol2000@gmail.com)
	Nathan Senner (n.r.senner@rug.nl)
	Andrew Johnson
	Johanna Perz
	Laura Koloski
	Laura McKinnon
	
Coats Island
	Paul Smith (PaulAllan.Smith@ec.gc.ca)

Colville
	David Ward (dward@usgs.gov)

East Bay
	Paul Smith (PaulAllan.Smith@ec.gc.ca)
	Grant Gilchrist

Igloolik
	Nicolas Lecomte (nicolas.lecomte@umoncton.ca)
	Marie-Andrée Giroux (marie.a.giroux@gmail.com)

Lower Khatanga River
	Mikhail Soloviev (mikhail-soloviev@yandex.ru)

Mackenzie Delta
	Jennie Rausch (jennie.rausch@ec.gc.ca)
	Paul Woodard (paul.woodard@ec.gc.ca)

Nome
	Brett K. Sandercock (bsanderc@ksu.edu): study years 1993-1995, 2010-2014
	David B. Lank (dlank@sfu.ca): study years 1996-1998, 2008-2013
	Willow English (willowenglish1@gmail.com): primary contact for Red-necked Phalarope data.
	Eunbi Kwon
	Samantha Franks
	Rick Lanctot

In addition to information that these authors might provide, it is likely that updates to the data will also be recorded at [Arctic Data Center](https://arcticdata.io).


4. Are there multiple versions of the dataset? 


## DATA-SPECIFIC INFORMATION FOR 'all_cover_fixed_JORGENSEN.csv':


1. Number of variables:

2. Number of cases/rows:

435 rows 

3. Variable List: <list variable name(s), description(s), unit(s)and value 
labels as appropriate for each>

4. Missing data codes: <list code/symbol and definition>

5. Specialized formats or other abbreviations used:

## SHARING/ACCESS INFORMATION

1. Licenses/restrictions placed on the data:

2. Links to publications that cite or use the data:

3. Links to other publicly accessible locations of the data:

4. Links/relationships to ancillary data sets: <any supplementary data sources 
that support analysis or classification of the datasets, eg., plant taxonomy table.)>

The data used in this project is hosted at the [Arctic Data Center](https://arcticdata.io). 

5. Was data derived from another source? If yes, list source(s): <list citations 
to original sources>

Data was not derived from another source

6. Recommended citation for the project:

When using the data and subsequent analysis for this project, the proper citation is: 

Lanctot, RB, SC Brown, and BK Sandercock. 2017. Arctic Shorebird Demographics Network. NSF Arctic Data Center.

























