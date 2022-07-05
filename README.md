![image](https://user-images.githubusercontent.com/60298572/177391195-b6cacc91-7db3-4ac0-ab3c-04242d64a94b.png)

**Background**
Holiday Helpers Canada is a philanthropic organization that delivers gifts to children in low-income neighborhoods. Christmas is a time of fun, but for families struggling to make ends meet with limited incomes, shelling out extra money for children’s gifts can be a challenge. 

That’s why Holiday Helpers Canada is motivated to bring a smile to the faces of children in low-income neighborhoods across Canada through this initiative. The gifts are generally dropped off outside the doors of households in low-income neighborhoods. However, they want to be able to effectively target children in need by identifying low-income neighborhoods in Canada. 

The organization found some data from Statistics Canada around household demographics but can’t find any income-related data for certain neighborhoods.  Therefore, they approached five Master of Management Analytics (MMA) students, who were more than willing to aid them with a clustering and predictive model to identify low-income neighborhoods based on a small dataset that mapped incomes to these household demographic metrics. 

Using the predictive model, the MMA students were determined to identify low-income census tracts for which only the household demographic data was available. 

**Results**
This project was completed by dividing the data into clusters using K-Means (further confirmed with Birch Clustering) to determine which household demographic characteristics are representative of the median income of neighborhoods. After determining the optimal number of clusters to be 4, the demographics of our target low-income cluster was as follows:
1.	Smaller household sizes which indicate smaller families
2.	The majority are living in apartment/condo buildings
3.	Higher rates of tenured ownership as opposed to renting
4.	The majority are living in older households built before 1980

Using these demographic characteristics, Holiday Helpers can successfully identify the census tracts containing the children in need, assuming they knew the household median incomes of the census tracts previously. If the household median income of the census tract is missing, however, then they can use the developed median household prediction algorithm. 

This prediction algorithm first clusters the census tracts based on known demographic data into low-income, medium-income, and high-income groupings (using a BIRCH algorithm), then uses a Random Forest Regressor to predict the median household income of the census tract.

Now Holiday Helpers Canada has a way to use demographic characteristics and median household income to identify which census tracts contain the highest number of children in need. As well, they can use the available census tract data demographic data to identify new low-income areas where the median household income was missing! Thus, Holiday Helpers Canada can successfully deliver presents and bring smiles to all the children in need!
