---
Post:
Title:  "local Weather Machine"
Date:   2018-02-16
Categories:

# Creating a local Weather Machine 

## Introduction 

FreeCodeCamp gave me a challenge to create a local weather App a project that i worked on for 3 days.

## Instruction 

 The app had to see the weather of my  current location.

It had to show  a different icon or background image (e.g. snowy mountain, hot desert) depending on the weather.

It had to also include a button to toggle between Fahrenheit and Celsius.

What was given was a API link https://fcc-weather-api.glitch.me . 

## solution

I started by getting the geolocation of my location by getting a freegeoip.net API . Which showed me my latitude and Longitude.The results
were then substituted to get The weather in that particular location. Substituting the Longitude and latitude allowed me to get different JSON object values which contended certain key value pairs for example icons for different weather conditions , Temperature in Celsius which i used to convert it into Fahrenheit using a certain formula. And What was left was creating the interface , which i used as a way to display the results.

## conclusion 

 The project was challenging , but fun doing this project gave me a better understanding of jquery and working with the get.JSON function.  




