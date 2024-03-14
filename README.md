# Climate-data_netCDF4-conversion
Data Extraction and Conversion from netCDF4 to Pandas DataFrame¶
This code extracts temperature (t2m) and total precipitation (tp) data from a netCDF4 file and converts it into a Pandas DataFrame. Here are the steps:

Import necessary libraries:

netCDF4: for working with netCDF files.
Pandas: for creating and manipulating DataFrames.
NumPy: for numerical operations.
Open the netCDF file and print its dimensions and variables.

Extract temperature (t2m) and total precipitation (tp) variables along with their attributes.

Extract scale factor and add offset for both temperature and total precipitation.

Convert time values to datetime objects using the num2date function.

Apply scale factor and add offset for temperature and total precipitation to obtain actual values.

Convert temperature from Kelvin to degrees Celsius.

Convert total precipitation from meters to millimeters.

Create arrays for latitude, longitude, and experiment version.

Create 2D arrays for latitude, longitude, and experiment version using meshgrid.

Flatten the 2D arrays for easier DataFrame creation.

Create a DataFrame containing time, latitude, longitude, experiment version, temperature (t2m), and total precipitation (tp) values.

Save the DataFrame to a CSV file named "climate_data_all_rows.csv".

Print a confirmation message indicating that the data has been saved successfully.
