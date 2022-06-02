11 464 car records scraped from Czech car dealership [AAA Auto](https://www.aaaauto.cz).

# Disclaimer

The scraped dataset was transformed with just some minor cleaning (mainly format fixes).
Due to this, there are some outliers and missing data, especially concerning expensive cars and the expiration date of STK. 

*Further cleaning is recommended!*

# Formats
* **Excel**
* **CSV**
* **JSON** - *Almost a raw scraped data. Includes lots of IDs and mainly a list of car equipment in acronyms.*

Example:
```
"equipment" : ["MSW","PS","TB","IF","AAC","ALL","ABS","PM","AB","CL","ESP","ASR","FG","ST","PW","COMP","XXX"]
```
# Columns

| Column | Data type | Description | Can be blank? |
| ------------- | ------------- |------------- |------------- |
| **price_czk**	| Single | *Price in CZK from 2/2022* | No |
| **brand**	| String | *Car brand* | No |
| **line**	| String | *Car model* | No |
| **bodywork**	| String | *Car body style*	| Yes |
| **transmission**	| String | *Type of transmission (Manual/Automatic)* | No |
| **number_of_gears**	| Single | *Number of transmission gears*	| Yes |
| **fuel**	| String | *Type of fuel used* | Yes |
| **year**	| Date (YYYY) | *Car model year* | No |
| **kilometers**	| Single | *Mileage (km)* | No | No | No |
| **engine**	| String | *Car engine*| No | No |
| **is_4x4**	| Boolean | *Is four-wheel drive vehicle?* | No |
| **power_kw**	| Single | *Car power output (kW)* | No |
| **size_ccm**	| Single | *Engine displacement (cm3)* | Yes |
| **doors**	| Single | *Number of doors* | No |
| **seats**	| Single | *Number of seats* | No |
| **color**	| String | *Car color* | Yes |
| **service_book** | Boolean | *Has service book?* | No |
| **stk**	| Boolean | *Has valid technical inspection?* | No |
| **stk_to**	| Date (MM/YYYY) | *Expiration date of technical inspection* | Yes |
