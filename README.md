# Anemia & Cancer Predisposition & Erythropoiesis

Several bone marrow failure syndromes have anemia as their major clinical feature. However, they have in common other things, most unexpectedly - significantly increased cancer predisposition. \
Cancer predisposition is linked to bone marrow failure syndrome, not to anemia in general. In this project, I am going to utilize some publicly available datasets on several anemias to investigate the specific fetures of bone marrow failure syndrome predisposition to cancer. \

* *Public datasets: load, QC, PP* are notebooks for **loading, quality control, and annotation of 5 single-cell RNA-Seq datasets** for Thalassemia, Sickle Cell Disease, Aplastic Anemia, Diamond-Blackfan Anemia, Fanconi Anemia, Myelodysplastic Syndrome (with 5q deletion). *Public datasets: integration* is a notebook for integration and batch correction. \
Initially, this was in one notebook, but it was too large to render it into GitHub as is and I had to split it. \
Celltypist and Azimuth we used for automatic annotation, followed by manual cluster-based annotation. \
Integration was two-step: unsupervised SCVI model on 1e4 HVGs was used to create the initial integration, and additional training was performed with supervised SCANVI model.
