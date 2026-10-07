# Awesome-Machine-Learning-Data-Preparation

## Top Machine Learning Data Preparation Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Data Cleaning, Feature Engineering & Self-Hosted Data Preparation*  

**Last updated: October 2026**



This repository tracks notable **commercial data preparation platforms** and **open-source projects** that clean, transform, and enrich datasets for machine learning — from visual data wrangling tools to automated feature engineering libraries and data quality frameworks.



**Examples** include Amazon SageMaker Data Wrangler, Alteryx Designer Cloud, Trifacta, Dataiku DSS, Databricks, Azure Data Factory Power Query, Coalesce, dbt Cloud, Tamr, and Prophecy.io (the category leaders).



**Open-source emphasis**: Data preparation is one of the strongest open-source domains in ML. **AKDATA** delivers enterprise-grade automated preprocessing with data leakage protection and health scoring. **Gators** brings 75+ Polars-based transformers from PayPal. **LeCrapaud** unifies feature engineering, selection, and hyperparameter optimization in a single `fit()` call. **OMR** provides comprehensive dataset quality validation and drift detection. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Amazon SageMaker Data Wrangler](https://aws.amazon.com/sagemaker/data-wrangler/)**  

  **AWS's visual data preparation tool** — 300+ built-in transformations with visual interface . **Feature Store integration and pipeline automation** . **Best for AWS-native data preparation** .



- **[Alteryx Designer Cloud](https://www.alteryx.com/)**  

  **The enterprise standard for visual data preparation** — drag-and-drop workflows with 300+ tools . **Best for enterprise data blending and analytics** .



- **[Trifacta (Alteryx)](https://www.trifacta.com/)**  

  **Cloud-native data wrangling** — machine learning-powered transformation suggestions . **Best for cloud data preparation** .



- **[Dataiku DSS](https://www.dataiku.com/)**  

  **Collaborative data science platform** — visual data prep, ML, and deployment . **Best for teams wanting visual and code-based workflows** .



- **[Databricks](https://www.databricks.com/)**  

  **Unified data and AI platform** — lakehouse architecture with data preparation capabilities . **Best for organizations using Spark and Delta Lake** .



- **[dbt Cloud](https://www.getdbt.com/)**  

  **Managed dbt platform** — SQL-based transformation with scheduling and documentation . **Best for analytics engineering** .



- **[Coalesce](https://coalesce.io/)**  

  **Data transformation platform** — column-aware SQL generation and automation . **Best for Snowflake-native data transformation** .



- **[Tamr](https://www.tamr.com/)**  

  **AI-powered data mastering** — entity resolution and data unification . **Best for master data management** .



- **[Prophecy.io](https://www.prophecy.io/)**  

  **Low-code data engineering** — visual pipeline builder for Apache Spark and SQL . **Best for Spark pipeline development** .



## Open-Source GitHub Projects



### Automated Data Preprocessing



- **[AKDATA](https://github.com/arikaranrs/AKDATA)**  

  **Enterprise-grade automated data preprocessing library**, open-source . **One-line API or modular pipelines** — detects missing values, removes duplicates, detects outliers, converts data types, encodes categoricals, generates features, selects features, splits train/test, scales numerics, and prevents data leakage . **Dataset Health Score (0-100)** based on missingness, duplicates, outliers, and type conflicts . **Data Leakage Protection** — automatically detects and flags target leakage before model training . **Fit-transform consistency** — computes statistics on training split and applies cleanly to test splits . **Automated HTML/PDF dashboards** with professional reports . **Best for production ML data preparation** .



- **[OMR (Omni Data Refinement)](https://pypi.org/project/omni-data-refinement/)**  

  **Pure Python framework for dataset quality, validation, and monitoring**, BSD-3-Clause licensed . **12 complete domains of data intelligence** — Health Engine (5-pillar quality score), Cleaning Engine (auto-resolution), Profiling Engine, Validation Engine (schema-based), Statistical Engine, Drift Engine (PSI, KS Test, JS Divergence), Monitoring System, Explainability, Versioning, Reporting, Pipelines, Plugin Registry . **Designed to be used immediately after loading a dataset**, similar to how Pandas is used for data manipulation . **Compatible with Pandas, Polars, and NumPy** . **No external AI APIs or LLMs required** . **Best for comprehensive data quality analysis** .



### Feature Engineering



- **[Gators](https://github.com/pspdatascience/gators)**  

  **Lightning-fast data preprocessing and feature engineering library from PayPal**, open-source . **Built on Polars** for multi-core parallel processing . **75+ preprocessing transformers** covering data cleaning, categorical encoding, numeric feature generation, string feature generation, datetime features, missing value imputation, and discretization . **sklearn-style `.fit()` and `.transform()` interface** — if you know sklearn, you already know Gators . **Production ready** — deploy the same Python code from notebook to production . **Comprehensive encoders**: CatBoostEncoder, TargetEncoder, WOEEncoder, LeaveOneOutEncoder, and more . **Advanced feature generation**: Fourier features, group lag features, ratio features, polynomial combinations . **Best for high-performance feature engineering** .



- **[LeCrapaud](https://pypi.org/project/lecrapaud/)**  

  **High-level Python library for end-to-end ML on tabular and time series data**, open-source . **Automated feature engineering** — Fourier dates, target encoding, imputation . **Ensemble feature selection** with 10+ methods and voting . **Hyperparameter optimization** — HyperOpt + Ray Tune . **Multi-target support** — native regression + classification . **Deep learning models** — LSTM, GRU, TCN, Transformer . **Time series support** — Fourier features, temporal CV, RNNs . **Explainability** — SHAP + LIME + feature importance . **Experiment tracking** — full artifacts in PostgreSQL/MySQL . **All in one `fit()` call** while remaining transparent and customizable . **Best for complete ML workflows** .



### Data Quality & Validation



- **[SanitiPy](https://pypi.org/project/sanitify/)**  

  **Intelligent data quality analysis and ML-assisted data cleaning**, open-source . **Structured dataset profiling** — schema-aware with scalable sampling . **Rule-based quality validation engine** with explainable weighted scoring . **Deterministic cleaning operations** — no hidden mutations, data is never altered silently . **ML-assisted fix suggestions** — confidence-scored, never auto-applied, human-in-the-loop by design . **Structured JSON report export** . **Production-oriented architecture** with test coverage . **Best for production data quality workflows** .



- **[Desbordante](https://github.com/desbordante/desbordante-core)**  

  **High-performance data profiler and cleaning tool**, open-source with **1,000+ GitHub stars** . **Discovers many different patterns in data** using various algorithms . **Allows running data cleaning scenarios** using discovered patterns . **Console version and easy-to-use web application** . **Best for pattern discovery and data profiling** .



- **[Cleanlab](https://github.com/cleanlab/cleanlab)**  

  **Data-centric AI library for label error detection**, open-source with **9,000+ GitHub stars** . **Implements confident learning framework** — iteratively refines label noise estimates by comparing model predictions with estimated label probabilities . **Active learning optimization** — selects most impactful examples for labeling . **Outlier detection** — identifies atypical data points . **Best for label quality improvement** .



- **[Great Expectations](https://github.com/great-expectations/great_expectations)**  

  **Data validation framework**, Apache-2.0 licensed with **9,000+ GitHub stars** . **Declarative data quality rules** — validate, document, and profile data . **Integrates with data pipelines** . **Best for data validation in production** .



### Data Curation & Versioning



- **[Argilla](https://github.com/argilla-io/argilla)**  

  **Collaborative AI feedback and data curation platform**, Apache-2.0 licensed with **3,000+ GitHub stars** . **Human-in-the-loop dataset platform** — coordinate annotators and domain experts . **Focus on LLM dataset curation and RLHF workflows** . **Best for LLM data preparation** .



- **[Hugging Face Datasets](https://github.com/huggingface/datasets)**  

  **Library for managing and processing large-scale ML datasets**, Apache-2.0 licensed with **19,000+ GitHub stars** . **Memory-mapped file access and lazy streaming** — handles datasets exceeding system memory . **Versioning and reproducibility** . **Best for large-scale dataset management** .



- **[Data-Juicer](https://github.com/modelscope/data-juicer)**  

  **Distributed framework for cleaning and transforming multimodal datasets**, Apache-2.0 licensed with **5,000+ GitHub stars** . **YAML-based data recipes** for reproducible pipelines . **Handles billions of samples** with Ray clusters . **Best for LLM and vision dataset preparation** .



- **[OpenRefine](https://github.com/OpenRefine/OpenRefine)**  

  **General-purpose data cleaning and wrangling platform**, BSD-3-Clause licensed with **11,000+ GitHub stars** . **Web-based interface with faceting and clustering** . **Reconciliation engine for entity standardization** . **Best for interactive data cleaning** .



### Additional Strong Open-Source Options



- **PrePro Auto** — Automated data cleaning with human-in-the-loop decision cards and versioning .

- **dsbro** — Notebook-heavy data science toolkit for fast EDA and baseline models .

- **Deesseia** — Unified data science toolkit from prototype to production .

- **Athena** — ML diagnostics platform with leakage detection and preprocessing script export .

- **Beaver FE** — Automated feature engineering with Bayesian optimization .

- **Pandas** — The foundational data manipulation library .

- **Polars** — Fast DataFrame library in Rust .

- **Dask** — Parallel computing for larger-than-memory datasets .

- **Apache Spark** — Distributed data processing for big data .



**Frameworks for building custom data preparation solutions**: Combine **AKDATA** for automated preprocessing with leakage protection and health scoring . Use **Gators** for high-performance feature engineering on Polars . Deploy **LeCrapaud** for end-to-end ML with automated feature engineering and hyperparameter optimization . Choose **OMR** or **SanitiPy** for comprehensive data quality analysis and validation . Integrate **Desbordante** for pattern discovery or **Cleanlab** for label error detection . Use **Hugging Face Datasets** or **Data-Juicer** for large-scale dataset management . Note that true enterprise data preparation with visual interfaces, collaboration features, and vendor-supported SLAs (SageMaker Data Wrangler, Alteryx, Dataiku) remains primarily commercial territory; open-source stacks provide strong automated preprocessing, feature engineering, and data quality foundations that require integration for complete data preparation platforms.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Data preparation platforms handle sensitive training data and may process PII. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **Data leakage is the most common ML bug** — AKDATA and SanitiPy provide automated leakage detection, but manual review is still essential . Target leakage produces overoptimistic validation metrics and poor production performance.

- **License considerations**: AKDATA is open-source , OMR uses BSD-3-Clause , Gators is open-source , LeCrapaud is open-source , and SanitiPy is open-source . Verify licensing against your use case before committing.

- The open-source ecosystem provides strong automated preprocessing, feature engineering, and data quality foundations, but **visual interfaces, collaboration features, and vendor-supported SLAs** remain primarily commercial offerings.



---



**Made for ML engineers, data scientists, and organizations seeking data preparation sovereignty.**

Let's make machine learning data preparation more open, transparent, and automated.
