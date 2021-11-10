# Ebay: Web-Scraping

The course project can be found [here](https://github.com/mikeizbicki/cmc-csci040/tree/2021fall/hw_03)

## What does the ebay-dl.py file do? ##
This program scrapes data from ebay for any search item. In particular, this program runs through the first 10 pages of ebay for the search item that is plugged into the terminal. The output is a JSON or a csv file that contains the name and price of the item, the item status, shipping cost and the return policy of the item.

### How to run the ebay-dl.py file - Generating a JSON file ###

First, to access the ``` ebay-dl.py ``` file, it will need to be downloaded from this repository. We then open up the file in vscode. To run the file, we write ``` $ python3 ebay-dl.py 'sandals' --num_page=10 ```. Here, 'sandals' can be replaced by any search item of your choice. This above code searches for the item plugged in the terminal, in this case sandals, across ebay. The desired results come out as a JSON file called ```sandals.json```. This also works for search items with a space, for example ```comic books, high heels```. To run this we can similarly write ``` $ python3 ebay-dl.py 'high+heels' --num_page=10 ```. The ```--num_page=10 ``` scrapes results from the first 10 pages of ebay when the item is searched up. If we want data scraped from the first 2 pages (or any other page) we can change ```--num_page=2```.
This is how I generated my JSON files called ```sandals.json```, ```screwdriver.json``` and ```comic+books.json```

### Generating a CSV file ###

To generate a csv file, we write ``` $ python3 ebay-dl.py 'sandals' --num_page=10 --csv h``` in the terminal. Compared to generating the JSON file, the addition here is the ``` --csv h ``` flag. This generates a csv file called ```sandals.csv```. This code tells the program to generate a csv file instead of a JSON. A term needs to be written after the ```--csv h``` to generate the csv file. Here 'h' is that term. However, any term can replace 'h'. It could be any word or letter or anything random.

