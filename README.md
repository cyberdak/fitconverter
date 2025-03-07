# GPS File Format Converter

A Python utility for converting GPS track data between different file formats, with a focus on .FIT file generation.

## Features

- Converts GPS track data from TCX and GPX formats to FIT format
- Handles coordinate conversions (degrees to semicircles)
- Calculates distances between track points
- Supports standard GPS data fields
- Generates valid FIT files with proper checksums

## Functions

The tool provides several key functions:

- `degree_to_semicircle()`: Converts GPS coordinates from degrees to semicircle format
- `distance_ll()`: Calculates distance between two lat/long points
- `step_tcx()`: Processes TCX format track data
- `step_gpx()`: Processes GPX format track data
- `write_field()`: Writes data fields to FIT format
- `checksum()`: Generates and validates FIT file checksums

## Usage

```python
# Example usage (converting TCX to FIT)
from write_fit import step_tcx

# Process TCX data
track_data = step_tcx(input_data)

# Write to FIT format
write_field(...)
```

## Requirements

- Python 3.x
- No external dependencies required

## License

This project is licensed under the terms included in the COPYING file.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

Thanks to all contributors who have helped with the development of this tool.
