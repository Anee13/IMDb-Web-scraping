# IMDb-Web-scraping

In this Python code uses web scraping techniques to extract movie data from IMDb for a specified genre. The code uses the BeautifulSoup library to parse the HTML content of the IMDb search results page, and the requests library to send HTTP requests to the IMDb website.

#Step 1: Importing the necessary libraries
The first step is to import the necessary libraries, which are requests and BeautifulSoup.


#Step 2: Specifying the URL and parameters for the IMDb search
The next step is to specify the URL for the IMDb search results page, and the parameters for the search. In this example, we are searching for crime movies, and we want the results sorted by user rating in descending order.


#Step 3: Sending an HTTP request and getting the response
The code then sends an HTTP GET request to the specified URL, passing the search parameters as a query string. The response is stored in a variable called response.


#Step 4: Parsing the HTML content of the response
The HTML content of the response is then parsed using the BeautifulSoup library. The BeautifulSoup constructor takes two arguments: the HTML content, and the parser to use. In this case, we are using the built-in HTML parser.


#Step 5: Finding the movie titles, stars, summarized movie, release date, writer and director
The code then finds the movie titles, stars, summarized movie, release date, writer and director using the find_all() method of the BeautifulSoup object. Each movie result is represented by a <div> element with the class lister-item-content.
For each movie result, we can then find the title, stars, summarized movie, release date, writer and director by searching for the relevant HTML elements within the <div> element.


#Step 6: Displaying the results in a table format
Finally, the results are displayed in a table format using the prettytable library. We first create a PrettyTable object and add the required columns, and then iterate over the movie results and add each row to the table.
