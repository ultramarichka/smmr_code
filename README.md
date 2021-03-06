# Reference-free error estimation for multiple multiple measurement methods
Code and data used in the article **"Reference-free error estimation for multiple measurement methods"** ([doi/10.1177/0962280217754231](http://journals.sagepub.com/doi/10.1177/0962280217754231)).

Documentation pending. If you want to speed things up, please ping me by raising
an issue.

To start sampling (provided you have pymc3 installed) adjust config.py to match
the dataset filenames and run sample.py. The trace is then saved in an .npy
file with the suffix "trace".

Use analyze.py to generate estimates and plots. It will make a separate folder with name matching 'config.py'. 
Please set `enable_logging` to False if you want to debug this file.

Use modesplit.py to reproduce separate mode analysis in the article.
Please set enable_logging to False if you want to debug this file.

Use 'lse_from_gen.py' to generate least squares estimates. Set `truth_source_suffix` to
'lse' in analyse.py and modesplit.py to compare to these estimates.

The clinical dataset ('20170710_0_*') uses cubic millimeters as units, use
'cubic_mm_to_cubic_cm.py' for conversion (run only once).

