---
title: MINC file format
author: yo3nglau
date: '2023-05-22'
categories:
  - Technical Blogs
toc: true
---

## TLDR

The MINC refers to a specific **file format** and **toolbox** dealing with multiple file formats from varying scanners and research groups.

## Description

The MINC file format and toolbox was originally conceived, written and released by Peter Neelin in 1992 due to the frustrations of dealing with multiple file formats from varying scanners and research groups.

In the ensuing years many associated tools (image registration, normalization, visualization, etc.) were written and have also been released. The original MINC file format and tools were based upon the NetCDF data format but problems were being encountered with multi-gigabyte datasets, as such a large rewrite of the library was undertaken in 2003 in which the data format was changed to HDF in order to support large files and other new features, resulting in MINC2. Development work on MINC1 was halted at version 1.5.1 in 2006. The current MINC2 library and tools are maintained by a group of developers in various image research labs around the world.

Another development effort, called the [MINC toolkit](http://bic-mni.github.io/), lead by Dr Vladimir Fonov, based solely on the MINC2 library (which can read MINC1 data). If you are new to MINC, it is suggested that you start here but keep in mind that this package is bleeding edge. The package was officially released on April 23 2012. This toolkit contains most of the commonly used MINC tools in one precompiled 64-bit binary package of Debian, Ubuntu and Mac OS X. Also contains interactive tools like register and Display, and some advanced tools such as patch-based segmentation, denoising and brain masking.

## Resources

https://www.mcgill.ca/bic/software/minc

https://en.wikibooks.org/wiki/MINC

http://bic-mni.github.io/