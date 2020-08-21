# Belly Button Biodiversity

![Bacteria by filterforge.com](Images/bacteria_by_filterforgedotcom.jpg)

Building an interactive dashboard to explore the [Belly Button Biodiversity DataSet](http://robdunnlab.com/projects/belly-button-biodiversity/).

Used Plotly.js to build interactive charts. 

Specifically, I created  a Pie chart that uses data from the  samples route (`/samples/<sample>`) to display the top 10 samples. 
   * Used `sample_values` as the values for the PIE chart
   
   * Used `otu_ids` as the labels for the pie chart
   
   * used  `otu_labels` as the hovertext for the chart.

  ![PIE Chart](Images/pie_chart.png)

I also created a Bubble Chart that uses data from the samples route (`/samples/<sample>`) to display each sample.

  * Used `otu_ids` for the x values

  * Used `sample_values` for the y values

  * Used `sample_values` for the marker size

  * Used `otu_ids` for the marker colors

  * Used `otu_labels` for the text values

  ![Bubble Chart](Images/bubble_chart.png)

Display the sample metadata from the route `/metadata/<sample>`

  * Displayed each key/value pair from the metadata JSON object somewhere on the page

 * All of the plots update any time that a new sample is selected.


Flask app is deployed to Heroku.
