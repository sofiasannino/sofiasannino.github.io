---
title: "Probabilistic Spatio-Temporal Modeling of Cardiac Deformation"
excerpt: "Defined a new probabilistic state-space model, representing cardiacmotion timeseries data by combining Gaussian primitives with Markovian Gaussian Processes<br/><img src='/images/sdsc_logo.png'>"
collection: portfolio
---
[📄 Report (PDF)](/files/Semester_project_Sannino_SDSC.pdf) | [💻 Code](https://github.com/sofiasannino/Cardiac-Deformation-SDSC)

In this work, we define the theoretical framework for a cardiac deformation model that
leverages temporal Gaussian process priors to correct control-points prediction on cardiac
volumes and make use of Gaussian splatting as rendering technique, to confront
predicted medical images and ground-truth.
Furthermore, we propose a geometry-based deterministic algorithm for efficient and accurate
control-points extraction from cardiac segmentation masks, to provide valid pseudo
ground-truth control points for the pre-training of the deformation model’s first stage,
a coordinate regression network.
Finally, we show the results of the training and inference experiments on the pre-training
of the coordinate regression network, conducted on the ACDC [1] dataset.
