# Satellite Positioning Data Processing

## Overview
This Python script efficiently propagates satellite positions over time using the SGP4 model, converting them to geographic coordinates and filtering based on predefined bounds. The script leverages multiprocessing for parallel execution, reducing computation time for processing a large number of satellites.

## Dependencies
- Python 3.x
- `sgp4` library (`pip install sgp4`)
- `pyproj` library (`pip install pyproj`)

## File Descriptions
1. `satellite_positioning.py`: Main Python script containing the implementation for satellite positioning and data processing.
2. `30000sats.txt`: Text file containing Two-Line Element (TLE) data for multiple satellites.
3. `error_log.txt`: Text file for logging any propagation errors encountered during the execution of the script.

## Usage
1. Ensure that Python and the required libraries (sgp4, pyproj) are installed.
2. Place the TLE data file (`30000sats.txt`) in the same directory as the script.
3. Run the script `satellite_positioning.py` using the command: `python satellite_positioning.py`.
4. The script will propagate satellite positions, convert them to geographic coordinates, filter based on predefined bounds, and log any errors encountered during the process.

## Customization
- Modify the `propagation_start_time`, `end_time`, `time_step`, and `bounds` parameters in the `main` function according to your requirements.
- Update the file paths for TLE data and error logging as needed.

## Output
- The script does not produce any output files by default. However, you can uncomment the code to write output data to CSV files (`output_file` variable in the `propagate_satellite` function).
- Processed satellite positions are logged in the console with information about the satellite name.

## Note
- Ensure that the system has sufficient computational resources to handle multiprocessing tasks efficiently.
- Verify that the provided TLE data file contains valid satellite information.
- Review the error log file (`error_log.txt`) for any propagation errors encountered during execution.

## Author
Abhishek Kumar

