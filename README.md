# MAGNIFinder
A software tool for 6-plex mdSUGAR tag labeled glycan peak pattern recognition automatically

This project is to find neutron coded pairs in MS1 spectra, as an cooperation project with Prof. Lingjun Li.
The peak detection algorithm and XIC construction algorithm are from our previously developed quantitative proteomics tool [PANDA](http://www.ncbi.nlm.nih.gov/pubmed/30816924)

## All the paramters were listed in the config file as follows:

CHANNEL_PLEX	6

//parameters for peak detection

MAX_CHARGE	4 //range: [2, MAX_CHARGE]

SN_CUTOFF	4

PEAK_RINT_CUTOFF	0	//minimum peak relative intensity

PEAK_INT_CUTOFF	0	//minimum peak absolute intensity

PEAK_TOLERANCE_PPM	5	//isotope peak mass tolerance: 5 ppm

//parameters between neutron-coded pairs

RT_TOLERANCE	5	//max rt range when merging redundant ions, default +/-5min

ION_TOLERANCE_PPM	5	//precursor ion tolerance when merging redundant ions, default +/-5 ppm

//raw files (one file per line)

d:/Tasks/Cooperations/mdSUGAR/07192022_ID8_mdSUGAR_2plex_R1.raw
