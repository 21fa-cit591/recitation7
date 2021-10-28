# Recitation 7
### October 28, 2021
## Topics to Recap
- File I/O
- Exceptions
- Git (remaining questions)

## Examples for Recap
- Implement a program that writes user input directly into a TXT file.

## Recitation Problem Set
### Preparation & Background
The material for this week's recitation are in a repository on GitHub. Your first task is to clone the repository into a new Eclipse project using  `File > Import... > Projects from Git (with smart import) > Clone URI`. 

When prompted for the repository's URI, use one of the following:
- https://github.com/21fa-cit591/recitation7.git
- git@github.com:21fa-cit591/recitation7.git

After you have successfully cloned the repository, please find the file ``StocksParser.java``. 

Once completed, this program will be able read from a CSV file containing stock price information and then store certain summary statistics into a TXT file. For this recitation, you will be using GameStop's stocks information from this year so far. This information has been provided in the file ``GME.csv``, which was downloaded from [Yahoo Finance](https://finance.yahoo.com/quote/GME/history?period1=1609718400&period2=1634860800&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true).

Note the following about CSV (Comma-Separated Values):
- CSV files are essentially data tables, in which each line is a row and columns are separated (i.e. *delimited*) by commas.
- The first line of a CSV file typically contains the column headers (for this program, we are interested in "Date" and "Close", *not "Adj Close"*)

After you have finished this assignment, you should be able to use this program on any "Historical Prices" information downloaded from Yahoo Finance.


### Program Requirements

Your job is to implement the following method of ``StocksParser``:

```
public static void processCSV(String inputFile, String outputFile)
```

This method should do the following:
1. Read from a CSV file ``inputFile`` (in this case, ``"GME.csv"``).
2. Parse out the following statistics:
   - The maximum closing price, and the date on which it occurred
   - The minimum closing price, and the date on which it occurred
   - The average closing price
   - The largest increase in the closing price in a single day, and the date on which it occurred.
   - The largest decrease in the closing price in a single day, and the date on which it occurred.
3. Write these statistics into ``outputFile`` (in this case, ``"stats.txt"``).

The output file should be formatted *exactly* as follows, starting on Line 1: 

```
Maximum: XXX.XX (YYYY-MM-DD)
Minimum: XX.XX (YYYY-MM-DD)
Average: XXX.XX
Largest Increase: XXX.XX (YYYY-MM-DD)
Largest Decrease: XXX.XX (YYYY-MM-DD)
```
* The actual value for the largest decrease should be negative, but you must print it as a positive number.


You may choose either of the following strategies:
1. Read the file and parse out the relevant data *before* finding the required statistics.
2. Find the required statistics 


## Submission
Please submit both ``StocksParser.java`` and ``stats.txt`` to Gradescope.

## NEW GROUPS:
Group # | Member 1 | Member 2 | Member 3 | Member 4
--------|----------|----------|----------|---------
Group 1 | Williams, Levester Randall | He, Ziyi | Cheema, Sardar Asfandy | Wu, Jeng-Ru
Group 2 | Cho, Suebin Grace | Kung, Ling-Hsin | Chheda, Shagun Pritesh | Arguello-Gonzalez, Marcos Abraham
Group 3 | Choi, Jae Ho | Qiu, Xi | Wang, Liujia | Kallas Jatene, Rafael
Group 4 | Ye, Huifang | Biscaro, Denise | Wang, Yuanqi | Qiu, Chengzhuo
Group 5 | Ng, Wai Chung | Lai, Qimei | Zhang, Han | Kong, Rachel
Group 6 | Hu, Yuxin | Bernat, Kevin Bruno | Chen, Zheyi | Wang, An-Jie
Group 7 | Pizzico, Tyler R | Shah, Rushabh | Lim, Xi Zhen | Xue, Mingxin
Group 8 | He, Donglun | Yiu, Hon-Cheung | Wang, Kehan | Pinheiro, Benjamin B
Group 9 | Huang, Wenyi | Zhang, Minzheng | Carnation, Kayla Rae | Guo, Zhaosen
Group 10 | Xiao, Zijian | Tims, George | Sha, Yumeng | Rigas, Andrew
Group 11 | Lee, Jaeyoung | Yu, Qingyu | Sabri, Rita | Patel, Rishi
Group 12 | Pace, Benjamin Michael | Liu, Jiayun | Bales, Elijah | Cai, Jialin
Group 13 | Li, Yunhe | Graham, Alexander Richard | Chou, Randy | Chen, Xiyue
Group 14 | Patel, Siddharth Bhagwanji | Zhang, Yang | Kim, Yunchae | Zhang, Yihong
Group 15 | Zhang, Miaoyan | Hu, Lucy Qian | Nojoomi, Radin | Sheng, Xinyue
Group 16 | Thenappan, Bala Sundar | Richmond, Christian | Nguyen, Tai D | Schnall, Aaron Hewitt
Group 17 | Liu, Shufan | Gallagher, John Manus | Jiang, Yao | Mammadov, Elmar
Group 18 | Liu, Xinyue | Ren, Yue | Zhang, Zhihui | Cruz, Marye I
