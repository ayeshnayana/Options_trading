# Options_trading
Options trading stratergy

# Data from Tradier.com
For this project, we're going to build an investing strategy that picks up options based on the highes change_precentatge. The trading date was obtained from tradier.com. The sandbox api is used to build the platform : https://sandbox.tradier.com/v1/ The config.py file containes the API_BASE_URL and ACCESS_TOKEN, which were not provided in the git repository. You need to create a developer/brocker account at tradier and obtain a API.

# Library Imports
Import pandas for the dataframe and request to retrieve data from the sandbox api. After creating the config file with your data import it as well. For this you need to save the file in the same directory.
Import the following libraries:
#requests
#pandas
#numpy

# Option analysis
After storing the option information into the dataframe we sort them by the highest change_precentatge of the option premium. In tradier.com the implied volatility is not provided at least in the free account. If you happen to know some other site which provides the implied volatility please let me know as well.

# Creating a Data Frame using the stock quotes
The data obtained for the stocks are filtered into averages and their standard deviations. The options data should be compared with historic averages, maximum and minimum quotes of the specific stock. In the descrpition_dataframe we find the daily average of the high prices and low prices. Then their standard deviations are also calculated. Maximum high value and the minimum low value is also filtered out. Any option strike which is higher than the maximum high and minimum low must be proceed with extra DD.
