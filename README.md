# CodeOptimisation_Digantara

##Dependencies:

Python 3.x
sgp4 library (pip install sgp4)
pyproj library (pip install pyproj)
File Descriptions:

satellite_positioning.py: Main Python script containing the implementation for satellite positioning and data processing.
30000sats.txt: Text file containing Two-Line Element (TLE) data for multiple satellites.
error_log.txt: Text file for logging any propagation errors encountered during the execution of the script.
##Usage:

Ensure that Python and the required libraries (sgp4, pyproj) are installed.
Place the TLE data file (30000sats.txt) in the same directory as the script.
Run the script satellite_positioning.py using the command: python satellite_positioning.py.
The script will propagate satellite positions, convert them to geographic coordinates, filter based on predefined bounds, and log any errors encountered during the process.
##Customization:

Modify the propagation_start_time, end_time, time_step, and bounds parameters in the main function according to your requirements.
Update the file paths for TLE data and error logging as needed.
