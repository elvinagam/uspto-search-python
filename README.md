# uspto-search-python
Searches USPTO database without API request

# Patent Search Script

This Python script uses the USPTO API to search for patents related to a given keyword. The results are then displayed in a formatted manner.

## Dependencies

The script requires the following Python libraries:

- `requests`: Used to send HTTP requests to the USPTO API.
- `textwrap3`: Used to format the output text.

## Usage

To use this script, simply run it with Python and provide a keyword as an argument.


This will display a list of patents related to "coca cola". Each patent includes the title, inventor names, publication date, abstract, and patent application number.

## Code Structure

The script defines a class `PatentSearch` with the following methods:

- `__init__`: Initializes the URL for the USPTO API.
- `wrap`: Formats a string to a specified width.
- `wrap_abstract`: Formats the abstract of a patent.
- `make_api_request`: Sends a GET request to the USPTO API and returns the JSON response.
- `search_and_display`: Searches for patents using a keyword and displays the results.

## Example Usage

Here's an example of how to use the script:

```
patent_search = PatentSearch()
input_text = "coca cola"
patent_search.search_and_display(input_text)
```
