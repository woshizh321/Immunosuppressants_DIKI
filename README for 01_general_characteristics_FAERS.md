This script assumes a single FAERS parquet that contains both case-level and drug-level fields (common in your pipeline). If you keep them separate, adapt the read_parquet() references accordingly.

Only PS/SS roles are counted to define exposure. We never rely on mixed role fields (e.g., ALL_DRUGS) unless you add a vetted PS+SS aggregate text field.
