---
layout: post
title:  "APL - Software Development Kit"
date:   2017-05-20
categories: blog
---
During my internship as a Software Engineer at the Johns Hopkins Applied Physics Laboratory I had the privilege to work on extending a Python package that parallelizes common data access workflows to allow for easy data transfer and analyses from different petascale databases through a single remote named `intern`. The software development kit (SDK) was actually developed for interactions with the Block Object Storage Service's (BOSS) RESTful API to allow for quick data access and analysis. However, the services `intern` provides were expanded to Janelia's DVID, another database mainly used to collect fly neurological data.

The tool went on to be heavily used by other interns to work on other projects as well as performers and clients of the BOSS database and DVID. Seeing as most of the SDK's users were scientists with little coding background, I lead a small team of engineers and scientists in the development of a user web-based interface that would allow for a more streamlined process. To combat the task, I used React-JS as the front-end element of the website and FlaskApp as the back end that executed all the commands required to perform the user's tasks. DVID's owner, Janelia soon began using the tool and their team is still using it today.

`intern` has become of big use in the academic industry as well, seeing as professors processing large amounts of data, prefer to streamline their data analysis with a single tool that can access multiple databases at the same time, while allowing for metadata updates and log entries. As a request from several clients I also worked on making an HDF5 designed local database to facilitate offline use and processing of data in a local machine without consuming as much space as it would to have the raw data stored locally without the HDF5 hierarchy.

The open source code for `intern` can be found [here](https://github.com/jhuapl-boss/intern).
