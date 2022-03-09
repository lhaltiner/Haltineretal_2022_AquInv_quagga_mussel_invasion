Data for: "The distribution and spread of quagga mussels in perialpine lakes north of the Alps"

Linda Haltiner, Hui Zhang, Orlane Anneville, Lukas De Ventura, J Tyrell DeWeber, John Hesselschwerdt,
Michael Koss, Serena Rasconi, Karl-Otto Rothhaupt, Roland Schick, Brigitte Schmidt, Piet Spaak,
Petra Teiber-Siessegger, Martin Wessels, Markus Zeh, Stuart R. Dennis
The distribution and spread of quagga mussels in perialpine lakes north of the Alps,
Aquatic Invasions, 2022,
https://doi.org/10.3391/ai.2022.17.2.02


 ######################################################################################################################

 Abstract: The dreissenid quagga Dreissena bugensis and zebra D. polymorpha mussels are invasive freshwater mussels in Europe and North America. These species strongly impact aquatic ecosystems, such as the food web through their high abundance, filtration rate. They spread quickly within and between waterbodies, and have the ability to colonize various substrates and depths. The zebra mussel invaded and established in Swiss lakes in the 1960s, whereas the quagga mussel was not detected until 2014. We collected all available data from cantonal as well as local authorities and other institutions to describe the colonization pattern of quagga mussels in Switzerland. We also collected data regarding the distribution of larval stages of the mussels, the so-called veliger larvae. We observed that in lakes colonized by the quagga mussel, veligers are present the whole year round, whereas they are absent in winter in lakes with only zebra mussels. Additionally, we present detailed information about the invasion and colonization pattern of quagga mussels in Lake Constance. Quagga mussels colonized the lakeshore within a few years (~ 2016-2018) and outcompeted zebra mussels, and have reached densities > 5000 ind. m-2 in the littoral zone, even at 80 m densities above 1000 ind. m-2 were found at some locations. At the end of the article, we discussed possibilities on how the spread of quagga mussels within and among northern perialpine lakes should be monitored and prevented in the future.

 Keywords: Dreissena density, Dreissena bugensis, veliger phenology, monitoring, Lake Constance, invasive species

######################################################################################################################

Contents:
README.txt (this file)
data.zip (contains datasets used in the paper in .txt format)
    BodenseeFewSelectedTribs_UTM.dbf
    BodenseeFewSelectedTribs_UTM.prj
    BodenseeFewSelectedTribs_UTM.qpj
    BodenseeFewSelectedTribs_UTM.shp
    BodenseeFewSelectedTribs_UTM.shx
    ConstanceShape_UTM.dbf
    ConstanceShape_UTM.prj
    ConstanceShape_UTM.qpj
    ConstanceShape_UTM.shp
    ConstanceShape_UTM.shx
    lakeconstance_depth_dreissena_sampling_2019.txt
    lakeconstance_depth_dreissena_sampling_2019_cv.txt
    lakeconstance_quagga_zebra_presence_absence.txt
    lakeconstance_quagga_zebra_proportions.txt
    veliger_data.txt

scripts.zip (contains the R code to generate figures and statistical analysis)
    Quagga_CH_Fig2_3_S2_veliger_data.R
    Quagga_CH_Fig4_LC_PresenceAbsence.R
    Quagga_CH_Fig5_LC_Quantitative.r
    Quagga_CH_Fig6_S3_Analysis.R

######################################################################################################################

README section for veliger densities


Data for Fig. 2, 3 and S2
data: veliger_data.csv
Rscript: Quagga_CH_Fig2_3_S2_veliger_data.R



This data set contains the veliger numbers (individuals/m3) for all veliger data of the research article.
Data from Lake Geneva can be downloaded an cited from:
Leslie Laine, Orlane Anneville, Serena Rasconi, Stuart R Dennis, Linda Haltiner
Time series dataset of mussels (Dreissena sp.) veligers densities in Lake Geneva from 2006 to 2019.
https://doi.org/10.15454/6D2BNU


Variables:
lake: which lake was sampled
site: where in the lake the sample is taken
source: who collected the data and provided it for this article
date: date of veliger collection
depthmin: in meters below surface, between which depths the sample was taken, e.g. 0, means, the sample was taken from the surface to the depth in the column depthmax
depthmax: in meters below surface, at which maximum depth the sample was taken, e.g. 60 means, the sample was taken from 60m to the depth in the deptmin column, integrated sample or sample at 1 depth
ind_m3: number of veligers per m3
quagga_present: adult quagga mussels present at this date
type: inlet or pelagic, inlet= sample was collected at an inlet pipe, pelagic= the sample was taken as an integrated sample in the middle of the lake


data provided by:
Veliger data for Lake Geneva was provided by OLA (Observatory on LAkes), Ã‚Â© OLA-IS, AnaEE-France, INRAE Thonon-les-Bains, CIPEL for IS OLA Data, https://doi.org/10.15454/6D2BNU
Zurich Water Supply, Hardhof 9, CH-8021 Zurich, Switzerland
Zweckverband Bodensee-Wasserversorgung, SÃƒÂ¼ssenmÃƒÂ¼hle, D-78354 Sipplingen, Germany
Ville de Lausanne, Service de l'eau, Rue de GenÃƒÂ¨ve 36,  CP 7416, 1002 Lausanne, Switzerland
Institut fÃƒÂ¼r Seenforschung, Landesanstalt fÃƒÂ¼r Umwelt (LUBW), Argenweg 50/1, 88085 Langenargen, Germany
Kanton Bern, BÃƒÂ¼ndackerstr. 44, 3047 Bremgarten, Switzerland




######################################################################################################################

README section of mussel density across depths of Lake Constance and coefficient of variation


Data for Fig. 6 and S3
data:
lakeconstance_depth_dreissena_sampling_2019.csv
lakeconstance_depth_dreissena_sampling_2019_cv.csv
Rscript: Quagga_CH_Fig6_S3_Analysis.R



We conducted depth monitoring in 2019 at 11 sites. At each site, we had 2 transects, where we did Ekman Grab samples (3 replicates)
at 3 depths where possible (30m, 60m and 80m).
in the Lower lake Constance part(=Untersee), we took grab samples at 10m and at maximum depth (varies between 20m and 45m depth).
This data set contains the densities of mussels (mussels/m2) per site.


lakeconstance_depth_dreissena_sampling_2019.csv
Variables:
date: date of the sampling day
lake: all in lake Constance, but split by the subparts, Untersee=lower LC, Obersee= Upper LC, Uberlingersee=Lake Uberlingen
site: name of the sampling site
transect: either 1 or 2, the transects are approximately 500m apart from each other.
depth: sampling depth with the ekman grab sampler
nr_grabsample: 3 replicated grab samples per depth
species: zebra or quagga
dreissena_nr: counts of Dreissenids per sampling area 0.0225m2
density: density of Dreissenids, mussels/m2
X: X coordinates
Y: y coordinates



lakeconstance_depth_dreissena_sampling_2019_cv.csv
This data set contains the coefficient of variation of each sampling site and depth.

Variables:
depth: sampling depth with the ekman grab sampler
site: name of the sampling site
lake: all in lake Constance, but split by the lake basins, Obersee= Upper LC, Uberlingersee=Lake Uberlingen
mean: counts of Dreissenids per sampling area 0.0225m2
sd: standard deviation
cv: coefficient of variation calculated as cv=sd/mean




######################################################################################################################

README section of quagga and zebra mussel occurrence in Lake Constance
lakeconstance_quagga_zebra_presence_absence.csv

Data for Fig. 4
data: lakeconstance_quagga_zebra_presence_absence.csv
Rscript: Quagga_CH_Fig4_LC_PresenceAbsence.R


This data set contains the binary anwers, if quagga or zebra mussels were present over the years (2016-2019) in Lake Constance


Variables:
region: part of Lake Constance (LC), Hochrhein= River High Rhine, Obersee= Upper LC, Uberlingersee=Lake Uberlingen, Untersee=Lowe LC
place: sampling place
site: sampling site
place_site: place and site combined and separated with a "_"
coordinates_lon_utm: longitudinal coordinates in UTM format
coordinates_lat_utm: latitudinal coordinates in UTM format
year: year of smapling
dbug_binary: 0 or 1, 0= no quagga mussels present at this site and year, 1= quagga mussels found at this site and year
dpoly_binary: 0 or 1, 0= no zebra mussels present at this site and year, 1= zebra mussels found at this site and year


data provided by:
Sampling was conducted by HYDRA (Konstanz, Germany) assigned by the International Commission for Lake Protection (IGKB)
and surveyed scientifically by the Institute for Lake Research, ISF, from the Landesanstalt fÃƒÂ¼r Umwelt Baden-WÃƒÂ¼rttemberg, LUBW in Langenargen (Germany).

######################################################################################################################

README section of quagga and zebra mussel proportions in Lake Constance


Data for Fig. 5
data: lakeconstance_quagga_zebra_proportions.csv
Rscript: Quagga_CH_Fig5_LC_Quantitative.R


This data set contains the proportions of quagga to zebra mussels over the years (2016-2019) in Lake Constance

Variables:
region: part of Lake Constance (LC), Hochrhein= River High Rhine, Obersee= Upper LC, Uberlingersee=Lake Uberlingen, Untersee=Lowe LC
place: sampling place
site: sampling site
coordinates_lon_utm: longitudinal coordinates in UTM format
coordinates_lat_utm: latitudinal coordinates in UTM format
year: year of smapling
month: month of sampling
season: season of sampling
dreis_m2_tot: number of Dreissena (zebra and quagga) per m2
proportion_Dbug: how many of the  mussels in dreis_m2_tot are quagga mussels, presented in %

data provided by:
Sampling was conducted by HYDRA (Konstanz, Germany) assigned by the International Commission for Lake Protection (IGKB)
and surveyed scientifically by the Institute for Lake Research, ISF, from the Landesanstalt fÃƒÂ¼r Umwelt Baden-WÃƒÂ¼rttemberg, LUBW in Langenargen (Germany).

######################################################################################################################


Cite as:
Data packages:

Linda Haltiner, Hui Zhang, Orlane Anneville, Lukas De Ventura, J Tyrell DeWeber, John Hesselschwerdt,
Michael Koss, Serena Rasconi, Karl-Otto Rothhaupt, Roland Schick, Brigitte Schmidt, Piet Spaak,
Petra Teiber-Siessegger, Martin Wessels, Markus Zeh, Stuart R. Dennis
Data for: "The distribution and spread of quagga mussels in perialpine lakes north of the Alps"
https://doi.org/10.25678/00052E

Leslie Laine, Orlane Anneville, Serena Rasconi, Stuart R Dennis, Linda Haltiner
Time series dataset of mussels (Dreissena sp.) veligers densities in Lake Geneva from 2006 to 2019.
https://doi.org/10.15454/6D2BNU


Paper:
Linda Haltiner, Hui Zhang, Orlane Anneville, Lukas De Ventura, J Tyrell DeWeber, John Hesselschwerdt,
Michael Koss, Serena Rasconi, Karl-Otto Rothhaupt, Roland Schick, Brigitte Schmidt, Piet Spaak,
Petra Teiber-Siessegger, Martin Wessels, Markus Zeh, Stuart R. Dennis
The distribution and spread of quagga mussels in perialpine lakes north of the Alps,
Aquatic Invasions, 2022,
https://doi.org/10.3391/ai.2022.17.2.02
