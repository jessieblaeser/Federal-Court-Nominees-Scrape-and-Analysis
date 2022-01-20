# Analyzing Fed Court Nominees via Pro Bono Work
 A scraper built to pull information from the Senate Judiciary Website. 
 
 This tool moves from the homepage of the Judiciary Committee to: 
* the meeting page 
* each past "Nominations" meeting
* click and download each questionnaire form for each nominnee presented in each nomination meeting 
* read and parse each PDF, checking for inconsistencies 
* using regex, pull key information from each PDF including, name, school, nominated position, pro bono work experience and more
* push this information into a Pandas dataframe
* download that information into a CSV

Using textual analysis, I've created a categorization system for the type of (required) pro bono work completed by those appointed to the federal courts. Examples of categories include things like: 
* Criminal Justice
* Child Protection 
* Discrimination and Human Rights 

The final output of this scraping project is a GeoJSON choropleth map that displays pro bono work categories by district. 
 
### Notebooks: 
* [Downloading nominee questionnaires](https://github.com/jessieblaeser/Federal-Court-Nominees-Scrape-and-Analysis/blob/233e10c37e2430277d0500f6941cc6e452ab3a04/Creating%20pro%20bono%20categories%20and%20mapping.ipynb): Using a combination of Beautiful Soup and Selenium, this notebook downloads over 50 PDFs from the Senate Judiciary Committee website. I use pdfminer to parse the PDFs and regex to pull information from each into a dataframe and CSV.
* [Creating pro bono categories and mapping](https://github.com/jessieblaeser/Federal-Court-Nominees-Scrape-and-Analysis/blob/233e10c37e2430277d0500f6941cc6e452ab3a04/Creating%20pro%20bono%20categories%20and%20mapping.ipynb): Using textual analysis, I categorize types of pro bono work, ultimately mapping the categories using GeoJSON. 

### Other uses: 

If you have no interest at all in pro bono work, this code can still be used to:
* Scrape the Senate Judiciary Committee's website
* Download specific files 
* Pool information about nominees 