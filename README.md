## WIGAB

Wigab is a Python library from parsing the Excel spreadsheets containing [election results](http://www.gab.wi.gov/elections-voting/results) produced by Wisconsin's Government Accountability Board. It currently returns a list of lists, with each element containing data that corresponds to one candidate result within a single jurisdiction (county or ward).

### Installation

Wigab should be installed by cloning this repository.

### Usage

In a Python shell, import the `process_all` function and supply it with a URL to an Excel file from the GAB site, along with a local file name:

```python
>>> from parser import process_all
>>> results = process_all("http://www.gab.wi.gov/sites/default/files/11.4.2014%20Election%20Results%20-%20all%20offices%20w%20x%20w%20report.xlsx", "2014_general_ward_results.xlsx")
```

### License

Wigab is released under the MIT License.
