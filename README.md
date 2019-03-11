# R_project
R project for CIS 585

# Utilize https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&filenum=000-22513&type=&dateb=&owner=exclude&start=40&count=40
# for Amazon.com's SEC database 10-k financial reports. Use Rvest in R to scrape the data from the website. Tidy the data and confirm its # usefulness.

## install the xlsx package first

install.packages("xlsx")

## next require the xlsx package

require(xlsx)

## read the excel sheet into a data frame

myfile <- "AmazonStats.xlsx"
xlsx_data <- read.xlsx2(myfile, sheetname = "sheet1")
class (xlsx_data)
head (xlsx_data)

## ERROR NOT UNDERSTANDING READ.XLSX2
