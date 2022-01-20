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
 