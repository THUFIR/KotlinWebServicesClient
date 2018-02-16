# KotlinWebServicesClient

consume wsdl

https://askubuntu.com/q/1006601/45156





$url = "http://www.webservicex.net/globalweather.asmx?wsdl"


$webservicex = New-WebServiceProxy -Uri $url -namespace WebServiceProxy -Class GlobalWeatherSoap


$webservicex | gm


echo $australiancities


$australiancities.NewDataSet


$australiancities.NewDataSet.Table



 $AustralianCities = $webservicex.GetCitiesByCountry("Australia")

echo $AustralianCities

echo "done"




but with kotlin..
