# Introduction

## Background

Prescribed drugs have side-effects. It can happen that a side-effect is triggered after the patient has started using the medicine. This side-effect can be recognized by a different doctor as a symptom of a new desease and a new prescription will be prescribed. This event is called prescription cascade. For pharmacist it is important to recognize these cascades and warn the doctors about this event, so the doctors can reconsider the medication and try to replace it with a similiar medicine.

MUMC+ is currently using a system which manages prescription of drugs to patients and will be replaced in following month by a new, more complex system. The system can detects possible overdose and conflicts between different drugs. The main issuse lies in a fact that the system cannot detect medical cascades. 

## Objectives

To enable the hospital spotting prescription cascades, new digital tool will be created to provide support to phamacists and doctors during medicine prescription. The goal is to provide an automatic solution which will use already known data about previous patitents and create warnings about possibility of a prescription cascades.

## Methodology

### Data collection

MUMC+ has a dataset of approximately 8 000 000 records in a relational database. These records will be provided as a csv file. Additional records could be downloaded from Dutch national register of drugs.

### Program development process

After the data will be obtained from MUMC+ data will be cleaned, unified and prepared for analysis. Then the PSSA analysis will be permormed. There is not a database of cascades so already known cascades can be rediscovered. There is an excellent chance to discover new cascades because the data provided by the hospital could reveal patterns which are not known today. Discovered cascades will be consultated with Yannick Nielen and other possible pharmacist which will provide expertise in this field and could point out the wanted and unwanted cascades. 

After the data analysis the digital tool will be created. Firstly a series of interviews and survey with potentional users will be conducted to capture feedback about the application functions. Also it is neccessary to get the information about possible layout of the application, how to warnings should be displayed and last but not least how to application would be used in production.

The draft of the product will be presented to Yannick Nielen and other pharmacist at MUMC+. This selection of people represents potentional users in the first phase of development. To tackle their ideas and comments series of code adjustment and presentation will be held. 

### Technologies

The data will be provided in a form of CSV file exported from a relational database. To extract useful information from the data Microsoft SQL Server database system will be used, which will provide the opportunity to query data via SQL.

Data analysis itself is going to be performed via Python. This includes libraries designed for data science, eg. Pandas, NumPy, Mathplotlib

Final digital tool will be written in ...... (Fill in when it will be known)

It is important to track changes made during software development, for this purpose Git will be used. To enable cooperation during member of the team, GitHub will be used.