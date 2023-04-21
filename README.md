# Voliboli

Welcome to our Web application for volleyball enthusiasts! Our platform offers a unique opportunity to analyze and compare volleyball statistics using visually appealing graphs. 
Whether you're a coach, player, or just a fan of the game, our platform provides valuable insights into player performance and team strategy. 
With the ability to upload your own match statistics in PDF format or search our database, you can easily access the information. 
Our user-friendly interface allows for easy navigation of the data, so you can focus on what's important - improving your game. 
Join our community today and take your volleyball analysis to the next level!

**Web page link:** [voliboli.lrk.si](https://voliboli.lrk.si/)

## Architecture

![Voliboli-arch (2)](https://user-images.githubusercontent.com/48418580/233632814-4b6c36d6-aa22-4492-8d75-b47bae6442dd.png)

## Main Features

- Automatically scraping statistics from [odbojka.si](https://odbojka.si/) using `Selenium`
- Scrape data of off PDF statistics document using `tabula-py`
- Store and retrieve data from `Flask` Backend using `GraphQL` with `Postgres` database configured as a persistest storage
- View and Analyze data on a WebPage created using `Streamlit`

## Components reference

- Web scraper code can be found in [WebScraping repository](https://github.com/Voliboli/WebScraping)
- PDF scraped code can be found in [PDFScraping repository](https://github.com/Voliboli/PDFscraping)
- Application backend code including Flask Server, GraphQL protocol and Postgres database interface can be found in [App-backend repository](https://github.com/Voliboli/App-backend)
- Application frontend code can be found in [App-frontend](https://github.com/Voliboli/App-frontend)
- In production this is running on Microk8s Kubernetes Cluster with pesistent storage and self-healing capabillities. Infrastructure configuration can be found [here](https://github.com/Voliboli/Infrastructure)