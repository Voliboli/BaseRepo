# Voliboli

Welcome to our Web application for volleyball enthusiasts! Our platform offers a unique opportunity to analyze and compare volleyball statistics using visually appealing graphs. 
Whether you're a coach, player, or just a fan of the game, our platform provides valuable insights into player performance and team strategy. 
With the ability to upload your own match statistics in PDF format or search our database, you can easily access the information. 
Our user-friendly interface allows for easy navigation of the data, so you can focus on what's important - improving your game. 
Join our community today and take your volleyball analysis to the next level!

## Architecture

![Voliboli-arch (2)](https://user-images.githubusercontent.com/48418580/233632814-4b6c36d6-aa22-4492-8d75-b47bae6442dd.png)

## Main Features

- Automatically scraping statistics from [odbojka.si](https://odbojka.si/) using Selenium
- Store and retrieve data from Flask Backend using GraphQL with Postgres database configured as a persistest storage
- View and Analyze data on a WebPage created using Streamlit
