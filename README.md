# Climate-data_netCDF4-conversion
# Data Extraction and Conversion from netCDF4 to Pandas DataFrame

This code extracts temperature (t2m) and total precipitation (tp) data from a netCDF4 file and converts it into a Pandas DataFrame. Here are the steps:

1. Import necessary libraries:
   - netCDF4: for working with netCDF files.
   - Pandas: for creating and manipulating DataFrames.
   - NumPy: for numerical operations.

2. Open the netCDF file and print its dimensions and variables.

3. Extract temperature (t2m) and total precipitation (tp) variables along with their attributes.

4. Extract scale factor and add offset for both temperature and total precipitation.

5. Convert time values to datetime objects using the num2date function.

6. Apply scale factor and add offset for temperature and total precipitation to obtain actual values.

7. Convert temperature from Kelvin to degrees Celsius.

8. Convert total precipitation from meters to millimeters.

9. Create arrays for latitude, longitude, and experiment version.

10. Create 2D arrays for latitude, longitude, and experiment version using meshgrid.

11. Flatten the 2D arrays for easier DataFrame creation.

12. Create a DataFrame containing time, latitude, longitude, experiment version, temperature (t2m), and total precipitation (tp) values.

13. Save the DataFrame to a CSV file named "climate_data_all_rows.csv".

14. Print a confirmation message indicating that the data has been saved successfully.

