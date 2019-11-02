---
layout: post
title: "Commmunity Bonding Period with FreeType"
modified:
categories: blog
comments: true
excerpt:
tags: []
image:
  feature:
date: 2018-05-15T00:00:00-00:00
modified: 2018-05-15T00:00:00-00:00
---
<p align='justify'>My proposal was selected for GSoC 2018 on 23 April. My project is "Integrating VFlib's TeX format drivers into FreeType". FreeType currently supports multiple font formats like truetype, opentype, bdf, pcf. My project aims to increase the supported formats by providing drivers for TeX's font formats (viz. GF, TFM, PK, and VF). Now, VFlib is a font library (no longer under development) which has a mature support for the above mentioned TeX font formats. I will be using the existing modules in VFlib as a reference to develop new modules for freetype on the lines of existing bitmap drivers already available in FreeType like BDF, PCF and WINFNTS.</p>
<p align='justify'>In the community bonding period I got acquainted with the workflow of the FreeType commuity. FreeType uses savannah to host their code for development and git as version control system. I initially set up my development environment, I was given the access to the savannah repository of FreeType. It was great fun to learn about savannah. In the process I had to learn about many advance git commands which I had not known earlier which were very useful and greatly simplified the development process. It was quite fascinating to know about how different modules can be compiled seperately from such a big library.</p>
<p align='justify'>Later I went through the source code of FreeType and learnt a lot of insights from the codebase and got my doubts cleared in the process. The community was very helpful in clearing my doubts. Specifically I learnt more about the current available drivers of BDF and PCF font formats and the working of their drivers. These drivers have many auxillary functions which facilitate the main functions, the object classes are defined very specific to the file format. I also learnt about the file structure followed by the drivers which simplifies and properly segregates the working code of the driver. This gave me an idea about how the new drivers can be designed more effectively.</p>
<p align='justify'>I am currently going through VFlib's codebase understanding some small intricacies of the drivers and subsequently started working on the code of GF Driver and will discuss about its working in the next blog post. Till then, Good Bye!!</p>
