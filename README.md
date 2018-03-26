# FlightPredictionML

Example of ML model implementation in VoltDB to predict delays in flights.
The library H2O is used to build the model since it's a market leader in machine learning and also provides the convenience of exporting models as Java code

Steps to run (assuming you have VoltDB and H2O installed)
1. Create a new flow or load a flow from h2o/ to start off a previously built model.
2. Train the model using your own data or data from data/ (using the H2O Flow UI or a language SDK)
3. Export the trained model as Java class.
4. Create a new stored procedure that accepts new events and calls the trained model class to make the predictions
