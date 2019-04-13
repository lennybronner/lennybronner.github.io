---
layout: post
title:  "Identifying the Higgs Boson"
date:   2019-04-10 22:23:10 -0400
categories: post
pic_folder: higgs
---

With guidance from Ariel Schwartzman and Ben Nachmen from the Stanford Linear Accelerator (SLAC) and the European Organization for Nuclear Research (CERN) I worked on using machine learning to help them identify the Higgs Boson from jet pull energy colourflow images.

Initially we tried using basic image processing techniques such as edge and corner detection together with conventional machine learning algorithms. Click [here](/assets/pdfs/cs229.pdf) to read more about this phase of the project. 

We later moved on to trying convolutional neural networks and other deep learning algorithms, which you can read more about [here](/assets/pdfs/cs231n.pdf).

This project was very successful. Our initial approach increased the testing AUC by 32% and in our final paper we achieved a 38% increased compared to the state of the art at the time.

We are currently in the process of trying to publish our results.
