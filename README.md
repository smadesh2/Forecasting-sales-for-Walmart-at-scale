Big Data analytics in the retail sector is enabling companies to create custom recommendations based on their purchase history thereby resulting in personalized shopping experiences and improved customer service. 

Specifically, we explore Walmart's weekly sales data with the below objectives -

 • Analyze past store sales data and identify key trends as well as factors that affect sales.
 
 • Develop an accurate forecasting tool to predict their stores’ sales for all the weeks on the planned horizon.

Our goal was to build hundreds of models and forecasts for each store-department combination, rather than a single forecast for the entire dataset, which would be extremely time-consuming to do as a sequential operation. We use Facebook's Prophet for forecasting and leverage the power of distributed programming in Spark, where individual worker nodes in a cluster can train a subset of models in parallel with other worker nodes, drastically lowering the time it takes to train the full collection of time-series models.
