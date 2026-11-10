---
title: "Language-Vision Deep Learning Model for Cancer Segmentation"
excerpt: "Designed a PyTorch vision-language lesion segmentation model on CT scans, fusing radiologist text embeddings (BERT) with image features.  <br/><img src='/images/logo_gustave_roussy.png'>"
collection: portfolio
---
[📄 Report (PDF)](/files/report_LSMS.pdf) | [💻 Code](https://github.com/sofiasannino/LVModel-Cancer-Segmentation)

Correctly identifying tumor lesions on Computed Tomography
(CT) scans is a crucial task in cancer diagnosis and treatment.
Developing and improving deep learning models to
automate tumor segmentation could significantly reduce diagnostic
errors and the time required to obtain a diagnosis.
To address this issues, we designed a comprehensive
pipeline for processing language–vision medical datasets
and a 3D vision–language segmentation model comprising
of a Language-Guided vision encoder with a Scale-aware Vision–
Language Attention module, a Full-scale decoder, and
a loss combining segmentation errors and contrastive errors.
We compare and validate our approach on a model previously
built at Gustave Roussy on abdominal CT scans with
liver cancer lesions.