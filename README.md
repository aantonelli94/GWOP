# GWOP


The gravitational-waves overlapping signals (**GWOP**) project aims at providing metrics to assess the biases on the parameters of a source of interest in the presence of confusion noise from other resolved or unresolved sources.

It is of relevance to 2G/3G ground-based detectors, and the spaceborne LISA mission. 

The repo contains three main folders:

- "Examples_ET" contains an implementation of an MCMC analyses for bias predictions using the PSD of ET, and a TaylorF2 model. The various examples include cases of increased complexity, starting from a simple implementation *without* potential sources of biases, to the case in which the signal is subject to detector noise, foreground noise, other resolved signals and waveform errors (the "global fit").

- "Examples_LISA" contains implementations using the LISA PSD, and a TaylorF2 model. The various examples include cases of increased complexity, starting from a simple implementation *without* potential sources of biases, to the case in which the signal is subject to detector noise, foreground noise, other resolved signals and waveform errors (the "global fit").

- "Explorations" contains various investigations on parameter inference biases with a foreground in LISA, when two signals coalesce close in time to one another, and when overlapping signals are resolved with incorrect waveform models.


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
