# Mutual-Fund-Peroformance-Analysis
Analyzed the performance of mutual fund scheme over the past 5 years. 
Mutual Fund Performance analysis

Introduction:

The aim of this project is to analyse the performance of open ended mutual funds over the past five years, and sort the top mutual funds on the basis of Sharp ratio in 10 different equity category.


Implementation details: -

•	Data extraction- Used BeautifulSoup for month wise data extraction from AMFI website for the last 5+ years from Jan 2017.

•	Data Storage- Stored data in default dictionary which is coming from AMFI website, and used other dictionary to store return of each month for every mutual fund which are listed on AMFI. Converted every mutual fund dictionary to CSV Stored in local memory.

•	Data cleaning- Clean the data of every mutual fund, dropped the mutual fund plans which had closed before June 2022. Filled all the empty data by linear interpolation.

•	Define attributes- Calculate the mean and variance of monthly returns for every plan of mutual funds and also calculated the Beta and Sharpe ratio.

•	Categorization- Categorized all mutual fund schemes in 10 different popular equity category like Large cap, Mid cap, small cap, flexi cap, Index fund, retirement fund, ELSS, Value fund, Focused fund and Dividend Yield fund. And also ranked in each category on the basis of Sharpe ratio and mean.

•	Performed an extensive literature review on risk and return analysis of Mutual Funds on the basis of parameters such as Beta, Treynor Ratio, Sharpe Ratio, Sortino Ratio, Jensens Alpha, Tracking error and IR Ratio



Library used:-

import requests- to get response
from bs4 import BeautifulSoup- to automate the data collection from AMIF website
from datetime import datetime, timedelta –for date and month and year
from collections import defaultdict - for storage of data
import csv 
import itertools - 
import pandas as pd – to perform analysis on collected data
import numpy as np - for mathematical help for performance  
from dateutil.relativedelta import relativedelta - to move one date to another date
import glob – iterate all the items(excel/csv) in a folder
from pathlib import Path
 

Conclusion: -

Using this project, we can track best performing mutual fund in different categories. From their Sharpe ratio we can find out that the mutual fund scheme is suitable for our risk profile. And we can get best performing Mutual Funds over the last 5 years in 10 different Equity Schemes.
