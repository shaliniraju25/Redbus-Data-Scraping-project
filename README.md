# Redbus-Data-Scraping-project

In this Redbus Data Scraping and Dynamic Filtering project, I've implemented a comprehensive solution that focuses on web scraping, data storage, and building a user-friendly interface for analyzing bus travel data across different states in India.

Why I Implemented This:

Purpose: 
The main goal is to make bus travel data more accessible and easier to navigate for users by centralizing the bus schedules, routes, fares, and availability from various states in India.

Problem Solved:
People often face challenges finding relevant bus information, especially across multiple state transport websites. This app provides a one-stop solution where users can filter buses based on their preferences like bus type, route, price, and more.


# How I Implemented This:

Data Scraping with Selenium:
I used Selenium to automate the extraction of bus details from the Redbus website, like bus names, routes, prices, seat availability, and timings.
Selenium interacts with dynamic web elements (like loading bus schedules) and pulls the data from Redbus into a structured format for further use.

Data Storage with MySQL:
After scraping, the data is stored in a MySQL database for persistent storage. This database allows for easy querying and filtering of data, ensuring that the user always sees the most up-to-date bus travel information.
MySQL also supports scaling, so as the data grows with more routes and states, the system can handle large volumes of information efficiently.

Dynamic Filtering and Frontend with Streamlit:
Streamlit is used to create an interactive web application where users can select bus details like routes, states, bus types, and more.
The filtering options allow users to get results in real-time, without needing to refresh the page or perform complex searches. The application dynamically pulls filtered data from MySQL based on the user's selections.

Rating Feature:
A rating feature allows users to rate the buses they traveled on, which is stored and updated in a CSV file for now (with future plans to move this to MySQL).
This feedback can be useful for other users to make informed decisions.


# What I Implemented:

Web Scraping:
Scraping dynamic content from Redbus using Selenium for multiple states and their routes.
Data for routes, fares, bus types, and timings were extracted across state-run bus corporations.

Database Integration:
The scraped data is then processed using Pandas and stored in MySQL for easy querying and filtering.
I also ensured that the data is cleaned and validated, particularly handling missing or incorrect price data using Pandas.

Interactive UI in Streamlit:
Users can filter buses by state, route, bus type, price, seat availability, and even departure time.
The UI is simple and intuitive, using drop-down menus, sliders, and time inputs to make navigation easy.

Rating System:
Users can rate buses after booking, and the rating is stored for future reference.
The application also calculates and shows the average bus rating.

Booking and Summary:
After choosing their route, users get a detailed booking summary that includes the state, route, travel date, departure time, number of passengers, fare, and rating. This enhances user experience by giving them all the information they need before finalizing the booking.


# Key Technologies Used:

Selenium: For web scraping dynamic content from Redbus.

Pandas: For data manipulation and cleaning.

MySQL: For efficient storage and querying of bus data.

Streamlit: For building the interactive front-end that allows real-time filtering and selection of bus routes.

CSV: Currently used for storing user ratings.



#####THANK YOU







