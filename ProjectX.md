<html> 
  <head> 
  </head> 
  
  <body>
  <h5> App Link </h5> 
  <a href = "https://vivekb.shinyapps.io/ProjectX/"> Shiny Apps Project X Link </a> 
  <br>
  <br>
  <div class = "description">
    <h3> Introduction and Description </h3> 
    <p> Project X is a project focused on learning how to develop shiny app web applications for data manipulation and visualization. However, Project X adds onto the concepts covered in Project 2 and Project3. Project X adds more complex graphing capabilities especially when it comes to maps. Some of the things covered within this app is learning how to import data, manipulate said data and then create a user interface for visualizing the data with leaflet maps. </p> 
    
   <br> 
    
   <p>  The project focuses on visualizing the energy that is used around the world and looking at the data over by region and production values. There is a focus on 15 resources overall: Coal, Hydro, Natural Gas, Oil, Wind, Biomass, Nuclear, Geothermal, Solar, Other, Waves and Tidal, Cogeneration, Petcoke. Storage, Waste. </p> 
   
   <br> 
   
   <p> The first page displays the power plantations around the world in the year 2019 and allows the user to toggle through the energies and see which plantations are more abundent and where they are located. </p> 
   
   <br> 
   <figure> 
    <img src="ProjectX_images/First_Page.png"> 
  <figcaption> A picture of the first tab that shows the Magellan Map and resources  </figcaption> 
  </figure>  
   
   <br> 
   
   <p>
   The graph is manipulatable and demonstrates a legend for each of the 15 unique sources. The graph allows the user to pan and see procedurally generated information. The map has a drop down to change the focus of the map onto a particular continent. The map can be adjusted by the generation output and the type of resource that you want to examine. Clicking on the type allows the user to see all plantations of that type around the world. The resource selection is able to select multiple resources. 
   </p>
   
  <br>
  <p> There is an about page on the second tab. </p> 
  </div>
  
  <br>
  <br>
  
  <div class = "data_description"> 
  <h3> Data Processing </h3> 
  <p> 
  The data was collected from the Global Power Plant Database featured at <a href = "datasets.wri.org"> datasets.wri.org </a>. The dataset details the information based off columns for each plantation. Each plantation is listed by the country code, country name, plantation name, plantation owner, location, production type, and production amount, followed by other background information such as development period, etc. 
  </p> 
  <br>
  <figure> 
    <img src="ProjectX_images/data_cleaning.png"> 
  <figcaption> A picture of the that shows the commands done to the dataset in R to clean the data</figcaption> 
  </figure> 
  <br>
  <p> 
    The initial data manipulation done to the dataset involved cleaning up the dataset such that it was easier to handle and more focused on the information trying to be collected.
  </p> 
  <br> 
  <p> 
    The first steps in cleaning up the data involved converting the dataset to the proper format. Converting numeric values from character to numeric was one of the first steps taken. The next thing to do was get the continent associated with each plantation based off the country code. There was some mislabels with countries like Kosovo. This was manually handled. 

</p> 

<br> 
<p> 
  Aside from that there weren't any other changes made to the dataset.
  </p> 
  <br> 
  
  </div> 
  
  <br> 
  <br> 
  
  <div class="instructions">
  <h3> Instructions to operate </h3>  
  <a href="https://github.com/Vivek2018/CS424ProjectX"> Github Project Repo </a> 
  <p> 
    To run this project there are a few requirements: <br> 
    1) Correct libraries and proper library versions
    2) Downloading the repo and opening the R project to start an R-Studio session
    3) Going to https://datasets.wri.org/dataset/globalpowerplantdatabase
    4) Downloading the data for 2019
  </p>
  <br> 
  <p> These instructions are enough to get the project working, however to make sure everything is compatable it is assumed that you have R-Studio and Shiny Apps already installed. Otherwise the user will need to install said software beforehand. There are a lot of libraries involved within the project so it is best to have everything up to date with this project. <br>

The libraries include: <br> 
library(shinydashboard) <br> 
library(shiny) <br> 
library(leaflet) <br> 
library(tidyverse) <br> 
library(hash) <br> 
library(countrycode) <br> 

  </p>
  </div>
  
  <br> 
  <br> 
  
  <div class="facts"> 
  <h3> Interesting Features </h3> 
  <p> 
    The data was an interesting analysis of what countries relied on and what the world relied on primarily for data generation. 
    </p> 
<br> 
  <p> 
    The most notable trends were focused around which country had the largest power plants and of what type they were. The initial assumption is that nuclear would be the largest generation source considering it powers somewhere from 10%-25% of the world's total power consumption. However when looking at the results from the 2019 the largest power plantations are from Hydro plantations based in China. 
  </p> 
  <figure> 
    <img src="ProjectX_images/interesting1.png"> 
  <figcaption> A picture displaying the largest plantations </figcaption> 
  </figure> 
  <p> 
    This result was based off by scaling the capacity of generation to about the upper half and there are only two plantations up in that fold. Both plantations are based in China and it seems the 3rd place ranked plantation is based on Gas in Russia but then again is overtaken by Hydro in South America. 
  </p> 
  <br> 

<figure> 
    <img src="ProjectX_images/interesting2.png"> 
  <figcaption> A picture displaying the largest plantations with expanded filters</figcaption> 
  </figure> 
  

  <p> 
    The basic conjecture looking at this is that Hydro is the largest producer for the world based off only the largest plantations. Looking at all plantations combined however and summing up their individual parts. 
  </p> 
  <br> 
  
  <p> If we do a cross comparison between all the types of resources that we know are the most heavily contributing: Coal, Gas, Hydro, and Nuclear we can compare the overall number and size to get an estimate on the number one contributing source around the world. </p>


  <figure> 
    <img src="ProjectX_images/coal.png"> 
  <figcaption> A picture of the coal data around the world</figcaption> 
  </figure> 
  <br>

  <figure> 
    <img src="ProjectX_images/gas.png"> 
  <figcaption> A picture of the coal data around the world</figcaption> 
  </figure> 
  <br>

  <figure> 
    <img src="ProjectX_images/hydro.png"> 
  <figcaption> A picture of the coal data around the world</figcaption> 
  </figure> 
  <br>

  <figure> 
    <img src="ProjectX_images/nuclear.png"> 
  <figcaption> A picture of the coal data around the world</figcaption> 
  </figure> 
  <br>
  
  <br>
  <br>
  <p> 
    Examining the results from the pictures it looks like a tie between coal and hydro. Both have numerous clusters but hydro definitely has the larger clusters but maybe not as frequent throughout the globe.
  </p>
  <br> 

  </div> 
  <br>
  <br>
  <div class="video"> 
  <h3> Youtube Video </h3> 
  <a href="https://youtu.be/Rp689LJQxmU"> Youtube Video Link </a> 
  <br>
  <br>
  <iframe width="420" height="345" src="https://www.youtube.com/embed/Rp689LJQxmU">
  </iframe>
  </div>
  </body>
 </html>
