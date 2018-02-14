---
layout: default
---

# PrivacyNoticeExperiment

## Introduction

### Experiment Aims

* To show that well-structured and controlled metadata can be used to automatically build a functional privacy notice.

### Possible benefits

* Privacy notices are produced to an agreed standard that meets user needs and which become recognisable to users 
* Privacy notices can stored in a single repository (personal.data.gov.uk perhaps)
* Gives personal data owners a reason to document personal data/services using standardised metadata
* Reduces workload of data protection specialists - no longer have to craft notices on a case by case basis

### Approach

* This experiment has been built quickly using a simple GitHub pages/Jekyll implementation (apologies for the ugly templating)
* The [Privacy Notice page](PrivacyNotice12345) presents a Privacy Notice for a dataset that is auto-generated from a CSV file of metadata which can be viewed [Here](https://github.com/andjnewman/PrivacyNoticeExperiment/blob/master/_data/goatlicences.csv).
* Whilst this experiment portrays a dataset it may be more appropriate to structure privacy notices (and thus metadata) around services the user understands.
* All content on the privacy notice and csv is entirely fictional (it is not an example of a good privacy notice!).
* Text shown in **_italics_** on the privacy notice is automatically generated based on the CSV data or hard coded logic based on the CSV data. (In a real implementation hard coding would be minimised through use of controlled lists etc)

### Take a look...

[Click here to view the experimental privacy notice](PrivacyNotice12345)
