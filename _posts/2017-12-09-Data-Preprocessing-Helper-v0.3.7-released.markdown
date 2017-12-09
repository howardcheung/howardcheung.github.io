---
layout: post
title:  "Data Preprocessing Helper v0.3.7 released"
date:   2017-12-09 18:00:00 +0800
categories: ["Data Preprocessing Helper"]
comments: true
---

One of the users of the software reports that the software does not work correctly when the time interval in the new file is larger than ones in the original file. For example, when your new file documents data at 10:00, 10:30, 11:00, etc. while your original file records data at 10:01, 10:04, 10:15, 10:31, etc., the software only uses the data at 10:01 to estimate the value at 10:00 but not the data at 10:04 and 10:15. The bug is fixed now, and the newest version of the software is now v0.3.7.

If your work involves scenarios similar to this case, please use the newest version to process your data again.

You can find the details of the project at [Data Preprocessing Helper](https://howardcheung.github.io/data-preprocessing-helper/) and download the new release [here](https://github.com/howardcheung/data-preprocessing-helper/releases/tag/v0.3.6).
