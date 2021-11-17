# Web Scraping Steam games site

### Problem Background:
Steam is a popular video game digital distribution service where gamers view and download games of their interest. Due to the increase in E-Sports, there are a number of games which have caught the interest of youth of this generation. Steam is home to a million games which are both Free to Play as well as purchase to play including all new releases, their ratings, reviews etc.

### Objective:
Steam site uses an infinite scrolling page(similar to twitter) as shown below:
![image](https://user-images.githubusercontent.com/35566625/142236593-73fc6240-ed3f-42ba-b325-deba23776a21.png)

As we can see below, steam site loads the page to view more results when we scroll down:
![image](https://user-images.githubusercontent.com/35566625/142238139-acfe2ccc-d1e2-4849-ba34-05e7cfb64830.png)

Objective is to create a scraper that automatically scrolls the pages and extracts information.

### Data Dictionary:
Field	| Description
--- | --- 
Title | Name of the game
Price | Price of the game on Steam site
Release Date | Date released
Steam user Rating | Average user rating
Users Reviewed | Number of users reviewed
Steam link | Link to access the game
Platforms Supported | Platforms the game can run on

### Scraping infinite scrolling sites:
For scraping infinite scrolling sites, a selenium web driver can be used. Chrome driver is an excellent example of the same. But, it requires a software(chrome driver) to run. When initiated, provided the scroll count, the driver automatically opens up a web page and scrolls w.r.t the scroll count. Once done, it saves the data in a .html file. We can open the .html file with encoding specified and prettify the data to a variable. This variable acts the same as a single page scraped data but with data of all pages. Processing can be performed to extract required columns to form the dataset.

##### Please Note:
Due to limitation in time and computing power, only a sample has been extracted by this method and shown in the Jupyter file.
