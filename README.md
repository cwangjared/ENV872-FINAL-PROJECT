# ENV872-FINAL-PROJECT

## Summary
This is a repository created for the final project of ENV872 course, by Jared Wang. The project aims to explore if residents of different race are influenced differently by concentrated animal feeding operations (CAFOs) in North Carolina.

## Investigators
Chengyang (Jared) Wang
Master of Environmental Management, Candidate
Email: cw369@duke.edu

## Keywords
Concentrated animal feeding operation; gestational age; birth weight; kernel density

## Database Information
This project uses 1) NC household level demographic and birth outcome dataset in 2016 and 2) hog CAFO kernel density scores. Both datasets are used in and wrangled for the purpose of my Masters' Project. In this project, I take the dataset wrangled for my MP and modify it to make it fit this project.

The demographic and birth outcome dataset is obtained from the NC birth certificate dataset (confidential information excluded). The dataset include the following variables: birth weight, gestational age, infant sex, mother's age, prenatal BMI, smoking history, prenatal care index level, naternal race, and maternal education.

Kernel density score reflects relative impact of hog CAFOs on each houeshold (each household has a unique score). It is calculated from numbers of hog CAFOs in 5 mi radius region, animal count in each CAFO, and animal size in each CAFO. The computation is previously completed by the Kernel Density tool in ArcGIS, as a part of my MP. Results are previously merged with the birth certificate dataset (code included below).

Date of data access: Nov 2019

> data folder contains raw and processed folder.
>> raw: original crude data
>> processed: data wrangled for this project

> output: final report

> code: rmd files for data analysis and report crafting

## Metadata
Data file used for this project is "data/processed/birth.kernel.csv". It contains 11 variables:
BMI: no unit; numeric
gestational.age: weeks, numeric
birth.weight: kg; numeric
kernel.score: no unit; numeric, used to quantify impact of CAFOs
kernel.score.log: no unit; numeric, natural log of kernel.score
marital.status: married or single; factor
infant.sex: male or female; factor
mother.age: yr; numeric
education: four levels; factor
race: black, hispanic, white, and other; factor
prenatal.care: four levels; factor
