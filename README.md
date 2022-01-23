# Mission-to-Mars

##Overview

Robin's web app is looking good and functioning well, but she wants to add more polish to it. She had been admiring images of Mars’s hemispheres online and realized that the site is scraping-friendly. She would like to adjust the current web app to include all four of the hemisphere images. To do this,we will use BeautifulSoup and Splinter to scrape full-resolution images of Mars’s hemispheres and the titles of those images, store the scraped data on a Mongo database, use a web application to display the data, and alter the design of the web app to accommodate these images.

##What You're Creating:

This new assignment consists of three technical analyses. 

Deliverable 1: Scrape Full-Resolution Mars Hemisphere Images and Titles
Using BeautifulSoup and Splinter, we will scrape full-resolution images of Mars’s hemispheres and the titles of those images.
Use the DevTools to inspect the page for the proper elements to scrape. 
created a list to hold the .jpg image URL string and title for each hemisphere image.
wrote a code to retrieve the full-resolution image URL and title for each hemisphere image. The full-resolution image will have the .jpg extension.
Loop through the full-resolution image URL, click the link, find the Sample image anchor tag, and get the href.
Save the full-resolution image URL string as the value for the img_url key that will be stored in the dictionary you created from the Hint.
Save the hemisphere image title as the value for the title key that will be stored in the dictionary you created from the Hint.
Before getting the next image URL and title, add the dictionary with the image URL string and the hemisphere image title to the list you created in Step 2.
print the list of dictionary items.

![image](https://user-images.githubusercontent.com/93686963/150697926-4e86bd56-fc43-47b9-a981-bb41196c5414.png)


Deliverable 2: Update the Web App with Mars Hemisphere Images and Titles

Using your Python and HTML skills, we wil add the code we created in Deliverable 1 to your scraping.py file, update your Mongo database, and modify your index.html file so the webpage contains all the information you collected in this module as well as the full-resolution image and title for each hemisphere image.
In the def scrape_all() function in our scraping.py file, we created a new dictionary in the data dictionary to hold a list of dictionaries with the URL string and title of each hemisphere image.
Below the def mars_facts() function in the scraping.pyfile, created a function that will scrape the hemisphere data by using your code from the Mission_to_Mars_Challenge.py file. At the end of the function, return the scraped data as a list of dictionaries with the URL string and title of each hemisphere image.
Run the app.py file, then check your Mongo database to make sure that you are retrieving all of the data.
Modify the index.html file to access your database, and retrieve the img_url and title as you loop through the dictionary in the database using {% for hemisphere in mars.hemispheres %}. The dictionary in the mars hemispheres database is the dictionary that was created from the Hint after Step 3 in Deliverable 1
Run the app.py file, open the index.html file, and click the "Scrape New Data" button.

![hemis1](https://user-images.githubusercontent.com/93686963/150698010-e973eb59-7a5c-4bc7-a0e8-107240030d6a.PNG)


Deliverable 3: Add Bootstrap 3 Components

For this part of the Challenge, update your web app to make it mobile-responsive, and add two additional Bootstrap 3 components to make it stand out.

![Final Web Page](https://user-images.githubusercontent.com/93686963/150698074-9877f1fb-a4d1-441d-9e99-a9b10b985335.PNG)











