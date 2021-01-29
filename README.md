# GWOP_public

Repository with results supporting arXiv:

The repo contains three main folders:

- "Examples_ET" contains an implementation of an MCMC analyses and bias predictions from the formalism of the paper using the PSD of ET and a TaylorF2 model. More details in the folder.

- "Examples_LISA" contains an implementation for the LISA detector. This folder also contains the necessary ingredients to reproduce the results of Sec.5.3 of the paper. 

- "Explorations" contains the implementations of the LISA codes for the results of Sec.5.1 and 5.2.


All the codes use emcee, for which the relevant citation is the following:

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


If you find these codes useful in any way, shape or form, please consider citing this, 





(A lot of time goes into building them up. Citing is always appreciated :) )


**Acknowledgements**: I benefitted greatly from discussions with a number of people. First and foremost, thanks go to Ollie Burke for helping me set up the codes, for discussions during the implementations, help and Python functions along the way and generally for keeping up with me. Many thanks to Lorenzo Speri for providing an implementation of emcee for a toy model, which I used as the basis for everything in this repo. Thanks also to Michael Katz for his expert advice on emcee. Any flaws or shortcomings are entirely my fault.
