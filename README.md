# Cosmic-Colours-and-X-ray-Part-1

 This code ius a single, self-contained Python script (make_xwas_figs_tables.py)
that reproduces every figure and table cited in the
manuscript except the machine-learning benchmark.
Run it once from the project root; it will

create a tidy outputs/ folder hierarchy,

regenerate xwas_agn_clean.csv,

dump all LaTeX‐ready tables (.csv) under outputs/tables/,

save all publication-quality PNGs (300 dpi) under
outputs/figures/, and

emit one hypothesis_tests.csv with the Welch, Spearman,
robust-OLS, and Anderson–Darling results.

Dependencies
pandas, numpy, scipy, statsmodels, seaborn, matplotlib,
pingouin (for Anderson–Darling).
Install once:
pip install pandas numpy scipy statsmodels seaborn matplotlib pingouin

outputs/
├── xwas_agn_clean.csv
├── tables
│   ├── descriptive_stats.csv
│   ├── class_counts.csv
│   └── hypothesis_tests.csv
└── figures
    ├── hist_logLx_by_class.png
    ├── box_logLx_by_class.png
    ├── scatter_logLx_vs_z.png
    ├── scatter_logLx_vs_BR.png
    ├── hist_flux_by_class_log.png
    ├── pairplot_continuous_vars.png
    ├── welch_density.png
    ├── spearman_scatter.png
    ├── regression_fit.png
    └── flux_survival.png
