<html> 
  <head> 
  </head> 
  
  <body>
  <h5> App Link </h5> 
  <a href = "https://vivekb.shinyapps.io/Project1/"> Shiny Apps Project 1 Link </a> 
  <br>
  <br>
  <div class = "description">
    <h3> Introduction and Description </h3> 
    <p> Project 1 is a project focused on learning how to develop shiny app web applications for data manipulation and visualization. Some of the basic things covered within this app is learning how to import data, manipulate said data and then create a user interface for visualizing the data. </p> 
    
   <br> 
    
   <p>  The project focuses on visualizing the energy that is used within the US and looking at the data over time. There is a focus on 9 resources overall: Coal, Hydro, Natural Gas, Petroleum, Wind, Wood, Nuclear, Geothermal, and Solar. </p> 
   
   <br> 
   
   <p> The first page displays the totals for the US and shows the 9 energies over time. The energy sources can be selected to give a more comprehensive idea. </p> 
   
   <br> 
   
   <img src="First_Page.png"> 
   
   <br> 
   
   <p> The second page allows the user to interact with two different regions and they are allowed to choose energy sources to compare between. They are able to select the same location and compare the same source over time or different sources in the same time frame for instance. The user is also able to select two different energy sources, two different time periods, and two different locations for comparison. The data displayed shows box plots for change in time as well as contribution. There are line plots for growth over time and raw data for comparison as well. </p> 
   <br> 
   
   <img src="Second_Page.png"> 
   <br> 
   <p> Finally the user is allowed to compare two different energy sources and two different time periods looking at the US holistically.   </p>
    <br> 
    <img src="Third_Page.png"> 
  <br>
  <p> There is an about page on the fourth tab. </p> 
  </div>
  
  <br>
  <br>
  
  <div class = "data_description"> 
  <h3> Data Processing </h3> 
  <p> 
  The data was collected from the US Energy Information Administration. The dataset was the net generation of energy organized by State and Type of Producer over time. 
  </p> 
  <br> 
  <p> 
    The initial data manipulation done to the dataset involved cleaning up the dataset such that it was easier to handle and more focused on the information trying to be collected.
  </p> 
  <br> 
  <p> 
    The first steps in cleaning up the data involved converting the dataset to the proper format. In this case certain features such as the GENERATION column was read in as string where in actuality it was a numeric value used to measure the production amount for the data. The other columns were converted to be more friendly values by converting them to factors. 

</p> 

<br> 
<p> 
  The second step involved missing data and incorrectly labeled data. There was a lack of uniformity in the data specifically with the STATE column. There was an issue with the labeling of data pertaining to the US overall data. Some tuples were labeled with “US-TOTAL” in all caps. There was another case that was mixed cased “US-Total” which needed to be converted to the same uniform value. The issue with the missing data also stemmed from the STATE column where there NA values present in the column that needed to be corrected. 
  </p> 
  <br> 
  <p> 
  The final measure that was taken was the most important one: selecting what data to look at and keep. The project strived to look at Coal, Hydro, Natural Gas, Petroleum, Wind, Wood, Nuclear, Geothermal, and Solar forms of energy; so other types needed to be removed. 
    </p> 
  </div> 
  
  <br> 
  <br> 
  
  <div class="instructions">
  <h3> Instructions to operate </h3>  
  </div>
  
  <br> 
  <br> 
  
  <div class="facts"> 
  <h3> Interesting Features </h3> 
  </div> 
  </body>
 </html>
