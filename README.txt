Plugins-
Software: python3 jupyter notebook (.sh files run python3 jupyter notebooks)

Environments: conda 4.8.5, python 3.7.0


Dependencies-
Python Libraries: pandas 1.0.3, numpy 1.18.1, requests 2.24.0, json 2.0.9, datetime, random


Programs-

.sh files:

assign1.sh 
top level script that runs the entire assignment

neighbor-districts-modifier.sh
runs Q1_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q1_Asgn1.ipynb

case-generator.sh
runs Q2_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q2_Asgn1.ipynb

edge-generator.sh
runs Q3_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q3_Asgn1.ipynb

neighbor-generator.sh
runs Q4_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q4_Asgn1.ipynb

state-generator.sh
runs Q5_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q5_Asgn1.ipynb

zscore-generator.sh
runs Q6_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q6_Asgn1.ipynb

method-spot-generator.sh
runs Q7_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q7_Asgn1.ipynb

top-generator.sh
runs Q8_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q8_Asgn1.ipynb

Jupyter Notebook files:

Q1_Asgn1.ipynb
Input: neighbor-districts.json, COVID-19 api
Output: nieghbor-districts-modified.json

Q2_Asgn1.ipynb
Input: neighbor-districts-modified.json, COVID-19 api
Output: cases-week.csv, cases-month.csv, cases-overall.csv

Q3_Asgn1.ipynb
Input: neighbor-districts-modified.json
Output: edge-graph.csv

Q4_Asgn1.ipynb
Input: neighbor-districts-modified.json, cases-week.csv, cases-month.csv, cases-overall.csv
Output: neighbor-week.csv, neighbor-month.csv, neighbor-overall.csv

Q5_Asgn1.ipynb
Input: neighbor-districts-modified.json, cases-week.csv, cases-month.csv, cases-overall.csv, COVID-19 api
Output: state-week.csv, state-month.csv, state-overall.csv

Q6_Asgn1.ipynb
Input: cases-week.csv, cases-month.csv, cases-overall.csv, neighbor-week.csv, neighbor-month.csv, neighbor-overall.csv, state-week.csv, state-month.csv, state-overall.csv
Output: zscore-week.csv, zscore-month.csv, zscore-overall.csv

Q7_Asgn1.ipynb
Input: cases-week.csv, cases-month.csv, cases-overall.csv, neighbor-week.csv, neighbor-month.csv, neighbor-overall.csv, state-week.csv, state-month.csv, state-overall.csv
Output: method-spot-week.csv, method-spot-month.csv, method-spot-overall.csv

Q8_Asgn1.ipynb
Input: zscore-week.csv, zscore-month.csv, zscore-overall.csv
Output: top-week.csv, top-month.csv, top-overall.csv

How to use:
In order to run all programs sequentially, run the following command from the terminal-
bash assign1.sh 
