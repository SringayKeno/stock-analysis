# stock-analysis

## Overview of Project: Purpose and Background of Analysis.

Steve, who rencently graduated with his finance degree, has asked me to assist him on analysis of a handful of green energy stocks for his parent's, who will be his first client. Steve has created an Excel file containing the stock data he wants us to analyze. I will be using an extension in Excel built for automating tasks, called Visual Basic for Application (VBA). VBA is able to make calculations, and use complex logic to perform analysis on the stock data. I will do analysis on two measures of the stock; 1) how actively stock was traded (daily volume) and 2) percentage increase or decrease in price from the beginning to the end of the year (yearly return). Additionally, I used the VBA code to automate the analysis which in the future, will allow Steve to do analysis with any stock.


## Results: 
### Stock Performance Between 2017 and 2018

Only two of the twelve green stocks carried positive returns with them into 2018 from 2017 (images 2017 and 2018 below). Those were tickers RUN (83.95% return) and ENPH (81.92%).The total daily volume for both those stocks increased from 2017 to 2018. Stock ticker DQ, who Steve's parents originally wanted to look at dropped significanly in 2018 (-62.60%) from its 2017 return (199.45%). 

images 2017 and 2018

<img width="251" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/102890151/163652730-d0a415ff-9eda-4be0-875e-4f49bc178064.png"> <img width="251" alt="VBA_Challenge_2018" src="https://user-images.githubusercontent.com/102890151/163652733-780cc8b0-1566-49a1-a271-15054d7090ec.png">![Screenshot (23)](https://user-images.githubusercontent.com/102890151/163657288-a83b9b9b-6e7a-4d42-80ef-22326a615615.png)


### Method- Daily Volume

Analysis was completed on two measures of the stock. The first was daily volume (how actively stock was traded). If I sum up all of the daily volume for a ticker, I will have the yearly volume and a rough idea of how often it gets traded. To find the total daily volume, I looped through every row in the stock data worksheet and checked for the ticker. Once the ticker was identified, the daily volume for that ticker was then then added to the total volume for the same ticker (See line '"5a" below in code

![VBA_Challenge_Volume](https://user-images.githubusercontent.com/102890151/163655664-2c8e8c20-d6bd-4f81-966d-14a78e003515.png)

### Method- Yearly Return

The second measure used to analye the stock was yearly return (the percentage increase or decrease in price from the beginning to the end of the year). To do this calculation I need the tickers first closing price and last closing price. To find the first closing price I looped through all the rows of data. Checked if the current row is the first row of the tickers data. If it was, I then set the starting price to the closing price in the current row (5b in image below). For the ending price I did the same (5c in image)

![Screenshot (19)](https://user-images.githubusercontent.com/102890151/163656718-b2b8351a-7d68-4f6b-a79c-0a55d360bce4.png)

### Measuring Code Performance

Steve, wants to do more stock research and he wants to expand the dataset to include the entire stock market over the last few years. Although my current code works well for the twleve stocks we analyed, it might not work as well for thousands of stocks. So I edited or refactored the code to make it more efficient —by taking fewer steps, using less memory, or improving the logic of the code to make it easier for future users to read.

To get the amount of time it will take to run Steve’s stock analysis script, I needed to capture the start time and end time of the executed code. VBA does have a Timer function.

![VBA_Challenge_Timer](https://user-images.githubusercontent.com/102890151/163657346-392fd7c0-425e-4f7c-8693-442861bf0ebf.png)

The starting time function is placed after the input box so once the year for analysis is chosen, the timer starts. Similarily there is an end timer placed at the end of the process.


After the 

## Summary: 

### In a summary statement, address the following questions.
### What are the advantages or disadvantages of refactoring code?
### How do these pros and cons apply to refactoring the original VBA script?
