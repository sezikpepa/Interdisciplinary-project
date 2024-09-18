# Introduction

## Background

Prescribed drugs have side effects. A side effect can be triggered after the patient has started using the medicine. This side-effect can be recognized by a different doctor as a symptom of a new disease and a new prescription will be prescribed. This event is called a prescription cascade. For pharmacists it is important to recognize these cascades and warn the doctors about this event, so the doctors can reconsider the medication and try to replace it with a similar medicine.

MUMC+ is currently using a system that manages the prescription of drugs to patients and will be replaced in the following month by a new, more complex system. This system can detect possible overdoses and conflicts between different drugs. The main issue lies in the fact that the system cannot detect medical cascades. 

## Objectives

To enable the hospital to spot prescription cascades, a new digital tool will be created to provide support to pharmacists and doctors during medicine prescriptions. The goal is to provide an automatic solution which will use already-known data about previous patients and create warnings about the possibility of a prescription cascade.

## Methodology

### Data collection

MUMC+ has a dataset of approximately 8,000,000 records in a relational database. These records will be provided as a CSV file. Additional records could be downloaded from the Dutch National Register of Drugs.

### Program development process

After the data is obtained from MUMC+, data will be cleaned, unified and prepared for analysis. Then the PSSA analysis will be performed. There is not a database of cascades so already known cascades can be rediscovered. There is an excellent chance to discover new cascades because the data provided by the hospital could reveal patterns which are not known today. Discovered cascades will be consulted with Yannick Nielen and other possible pharmacists who will provide expertise in this field and could point out the wanted and unwanted cascades. 

After the data analysis, the digital tool will be created. Firstly a series of interviews and surveys with potential users will be conducted to capture feedback about the application functions. Also, it is necessary to get information about the possible layout of the application, how warnings should be displayed and last but not least how to application would be used in production.

The draft of the product will be presented to Yannick Nielen and other pharmacists at MUMC+. This selection of people represents potential users in the first phase of development. To tackle their ideas and comments series of code adjustments and presentations will be held. 

### Technologies

The data will be provided in the form of a CSV file exported from a relational database. To extract useful information from the data Microsoft SQL Server database system will be used, which will provide the opportunity to query data via SQL.

Data analysis itself is going to be performed via Python. This includes libraries designed for data science, eg. Pandas, NumPy, and Mathplotlib.

The final digital tool will be written in ...... Blazor? (Fill in when it will be known)

It is important to track changes made during software development, for this purpose, Git will be used. To enable cooperation among the members of the team, GitHub will be used.

### Ethical considerations

During the development of the digital tool, an analysis of medical data be conducted. Information about patients' health is personal information, so the data should not be shared with anybody to provide anonymity and confidentiality of people's data. The final digital tool cannot share data with third parties outside of MUMC+ hospital.

### Evaluation

Main users will be pharmacists so it will be up to them to decide about the quality of the application and their comments will be addressed to accommodate their needs.