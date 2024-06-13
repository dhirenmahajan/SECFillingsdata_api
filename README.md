   # Retrieve SEC Filings  
   
This project is a Python script that retrieves SEC filings for a given company ticker symbol. It uses HTTP GET requests to fetch the company's filing metadata from the SEC website and downloads the documents of interest (10-K and 10-Q forms).  
   
## Requirements  
   
- Python 3.6+  
- Python packages: requests, pandas, logging, os  
   
## Usage  
   
To use this script, simply call the `getCompanyFiles(ticker: str)` function with the ticker symbol of the company you are interested in. For example:  
   
```python  
getCompanyFiles('AAPL')  
```  
   
This will fetch the SEC filings for Apple Inc. and download the documents into a directory named 'AAPL'. If the directory does not exist, it will be created.  
   
## Error Handling  
   
The script has error handling in place for potential issues such as:  
   
- Network errors during HTTP requests  
- JSON parsing errors  
- Missing ticker symbol in the SEC's company tickers list  
   
All errors are logged to the console for easy debugging.  
   
## Note  
   
This script mimics a browser request to access the SEC website. Please use it responsibly to avoid overloading the SEC servers.
