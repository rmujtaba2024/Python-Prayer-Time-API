Daily Prayer Time API 
  
It's an easy to use API to get today's (and tomorrow!) prayer time     
Written in Python using _Flask, Beautiful Soup, and Google-Search-Python.  

To Print Data in Python:-      
import requests     
import json         
  
url = "https://dailyprayer.rmujtaba.repl.co/api/usa"    
response = requests.get(url)    
data = response.json() 
print(data['city'])   
print(data['date'])   
for prayer in data["today"]:   
  print(prayer + ": " + data["today"][prayer])      

 

Example Output: 
 
Singapore   
17 January 2021   
Fajr: 05:52   
Sunrise: 07:14   
Dhuhr: 13:17   
Asr: 16:40   
Maghrib: 19:17   
Isha'a: 20:30.   
