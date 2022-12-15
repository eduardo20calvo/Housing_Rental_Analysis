# Housing Rental Analysis

The purpose of this project is to use data visualizations, including aggregation, interactive visualizations and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities. Data includes the San Francisco Census Data over the years. Some of the tasks include calculating and plotting the housing units per year; calculating and plotting the average prices per square foot; comparing the average prices by neighborhood; building an interactive neighborhood map; and conclusion. The tools used in this analysis include Pandas, HvPlot and GeoViews. The main programming language used is Python.

## Calculate and Plot the Housing Units per Year

Once the data was imported and organized into a DataFrame, the dataset was grouped by year and aggregated by the mean. A graph was then used to plot the housing units per year:

![bokeh_plot2](https://user-images.githubusercontent.com/104874384/207756532-156291bf-f7fb-40e1-afe8-22312ccd3fea.png)

Based on the graph above, there is a positive trend as there is an increasing number of housing units each year.

## Calculate and Plot the Average Sale Prices per Square Foot

As per the previous task, the dataset was grouped by year and aggregated by the mean. The dataset was then filtered out to only include data for average sale price per foot and average gross rent. Based on the DataFrame, the lowest gross rent reported between the years is $1,239 in 2010. The prices per square foot by year and gross rent per year was plotted into the line graph below:

![bokeh_plot3](https://user-images.githubusercontent.com/104874384/207757513-ab000e76-6417-41b2-adc1-a1a8e7cbc44a.png)

Based on the graph above, there was a slight drop in average sale price per square foot in 2011. It is also observed that gross rent increased that year.

## Compare the Average Sale Prices by Neighborhood

Similar to previous tasks, the dataset was manipulated but this time, by grouping it by year and neighborhood and aggregating it by the mean. Then the housing units were filtered out to only include the average sale price per square foot and average gross rent. This data was plotted in the graph below:

![bokeh_plot4](https://user-images.githubusercontent.com/104874384/207758586-39e86c9a-1ecb-45ba-9f06-9e9800c118f1.png)

Based on the graph above, one observation we can make is that the average sale price per square foot in 2016 is less than the price that's listed for 2012 for the Anza Vista neighborhood.

## Build an Interactive Neighborhood Map

To prepare the interactive neighborhood map using HvPlot with GeoViews enabled, the csv file containing neighborhood coordinates was imported and organized into a DataFrame. The previous DataFrame containing the San Francisco Census Data was manipulated to be grouped by neighborhood and aggregated by the mean. These two DataFrames were then concatenated into one DataFrame. Last but not least, this dataset was used to plot the interactive neighborhood map using HvPlot enabled with GeoViews: 

![bokeh_plot5](https://user-images.githubusercontent.com/104874384/207761199-6fa1280a-c526-4f2e-b484-22f0442842cc.png)

Based on this interactive map, we can conclude that the neighborhood with the highest gross rent is Union Square while the neighborhood with the highest sale price per square foot is Western Addition.

## Conclusion

There seems to be a slight positive trend between the rental income growth and sale prices over the years, except for 2016 where as the rental income went up, the sale prices went down. The trend does not hold true for Union Square where rental income is not increasing as steadily. Speaking from the data contained in San Francisco, it makes sense to purchase houses for rent as the rent is going up at a faster rate than sale prices. Based on the data obtained, almost all the homes follow this trend. Bay View and Silver Terrace would be great neighborhoods to purchase as the rent is pretty high compared to sale prices.
