# GWOP

**Description**


The codes in this repository support the results in arXiv:2104.01897.

The codes in this repo investigate the situation in which multiple gravitational-waves overlapping signals (**GWOP**) are present in a GW data stream (a situation of relevance to 2G/3G ground-based detectors, and the spaceborne LISA mission). The aim is to provide metrics to assess the biases on the parameters of a source of interest in the presence of confusion noise from other resolved or unresolved sources.

The repo contains three main folders:

- "Examples_LISA" contains an implementation of an MCMC analyses for bias predictions using the PSD of LISA, and a TaylorF2 model. The various examples include cases of increased complexity, starting from a simple implementation *without* potential sources of biases, to the case in which the signal is subject to detector noise, foreground noise, other resolved signals and waveform errors (the "global fit").

- "Examples_ET" contains the same as above, but using ET's PSD.

- "Explorations" contains various investigations on parameter inference biases with a foreground in LISA, when two signals coalesce close in time to one another, and when overlapping signals are resolved with incorrect waveform models.


**You need**

All the codes in this repo are intended to be self-contained. You will still need to install the standard packages and emcee, for which one needs to run the following lines in the terminal

- `pip install scipy` 
- `pip install matplotlib`
- `pip install corner` (for corner plots)
- `pip install emcee` (These codes have been tested with emcee v3.0.2)
- `pip install tqdm` (This library is for the progress bar during the MCMC sampling)

**Please cite:**

If you have found the codes in this repository useful, please cite the paper they were developed for,

@article{Antonelli:2021vwg,
    author = "Antonelli, Andrea and Burke, Ollie and Gair, Jonathan R.",
    title = "{Noisy neighbours: inference biases from overlapping gravitational-wave signals}",
    eprint = "2104.01897",
    archivePrefix = "arXiv",
    primaryClass = "gr-qc",
    month = "4",
    year = "2021"
}

All the codes use emcee, for which the relevant citation is

@article{ForemanMackey:2012ig,
    author = "Foreman-Mackey, Daniel and Hogg, David W. and Lang, Dustin and Goodman, Jonathan",
    title = "{emcee: The MCMC Hammer}",
    eprint = "1202.3665",
    archivePrefix = "arXiv",
    primaryClass = "astro-ph.IM",
    doi = "10.1086/670067",
    journal = "Publ. Astron. Soc. Pac.",
    volume = "125",
    pages = "306--312",
    year = "2013"
}

**Acknowledgements**: for these codes, I benefitted greatly from discussions with a number of people. First and foremost, thanks go to Ollie Burke for helping me set up the codes, for discussions during the implementations, help and Python functions along the way and generally for putting up with me. Many thanks to Lorenzo Speri for providing an implementation of emcee for a toy model, which I used as the basis for everything in this repo. Thanks also to Michael Katz for his expert advice on emcee. Legally, I'm obliged to say that any flaws or shortcomings are entirely my fault (but they are probably Ollie’s). 

Please direct questions to `andrea.antonelli@aei.mpg.de` 
