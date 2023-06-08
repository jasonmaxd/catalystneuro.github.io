---
layout: single
title: "Axona Data Processing Columbia University"
categories: project
date: 2020-01-01
show_date: false
author: CatalystNeuro
classes: wide
type: project
role: NWB Specialist and Developer
---

The CatalystNeuro team worked with Dr. Hussaini and his lab to utilize a state-of-the-art preprocessing workflow on electrophysiological data collected as part of their research on Alzheimer’s Disease. Data was being collected from the Axona acquisition system and from Intan. They used MountainSort and were interested in comparing these results to other cutting-edge spike sorters and accelerating data processing through curation using spike train metrics, consensus across sorters, and finally manual curation. They wanted the output of this processing system to be capable of writing the results in TINT format. We built this system in SpikeInterface, a package designed to build modular spike sorting pipelines.