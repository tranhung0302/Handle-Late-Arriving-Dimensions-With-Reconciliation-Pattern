# Handle late-arriving dimensions with reconciliation pattern

Processing facts and dimensions is the core of data engineering. Fact and dimension tables appear in what is commonly known as Star Schema. In a data warehouse, a fact fact table is surrounded by one or more dimension tables as it holds a reference to dimension natural or surrogate keys.

In order to ensure the accuracy of the data, dimensions are ussually processed first as they need to be looked up while processing the fact. We are going to go through a few use cases of late-arriving demensions and potential solutions to handle it with a simple Spark pipeline.