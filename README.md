# Analyzing Fed Court Nominees via Pro Bono Work
 A scraper built to pull information from the Senate Judiciary Website. 
 
 This tool moves from the homepage of the Judiciary Committee to: 
* its meeting page --> 
* finds each past "Nominations" meeting --> 
* clicks and downloads each questionnaire form for each nominnee presented in each nomination meeting
* reads and parses each PDF, checking for inconsistencies  
* using regex, pulls key information from each PDF including, name, school, nominated position, pro bono work experience and more
* pushes this information into a Pandas dataframe
* downloads that information into a CSV

Using textual analysis, I've created a categorization system for the type of (required) pro bono work completed by those appointed to the federal courts. Examples of categories include things like: 
* Criminal Justice
* Child Protection 
* Discrimination and Human Rights 

The final output of this scraping project is a GeoJSON choropleth map that displays pro bono work categories by district. 
 