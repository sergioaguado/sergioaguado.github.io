---
title: "Spanish beaches"
author: "Sergio Aguado"
highlighter: highlight.js
output: html_document
job: null
knit: slidify::knit2slides
mode: selfcontained
hitheme: tomorrow
subtitle: One of the most important resources for attracting tourism
framework: io2012
widgets: shiny
---

## Introduction

In 2014, Spain was the second classified in the ranking of ["International tourism receipts"](http://dtxtq4w60xqpw.cloudfront.net/sites/all/files/pdf/unwto_barom15_02_april_excerpt__0.pdf). Culture, history, nature, sun are some of the things, that attract tourists from all over the world. But without any doubt, the Spanish beaches are the most important natural resource for the tourism sector.

This is study tries to describe the Spanish beaches: Length, width, vegetation, 
urbanization and occupation level, and other kind of equipments.

The data set used for this research is "Guía de playas" from the open data initiative from
the Spanish government. The data set has been translated in English because is the language of
this course. 

<br>
You can download the data set from [here](http://datos.gob.es/catalogo/guia-de-playas)

--- .class #id 
## Summary

Spain has 3.463 beaches shared in 12 Autonomous Communities with a total length of
1871.6 kilometers. But to make a better idea about the Spanis beaches and their 
equipments, take a look at the following table



<!-- Table generated in R 3.2.0 by googleVis 0.5.8 package -->
<!-- Sun Apr 26 20:55:53 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID3bb1cc36441 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Blue flag*",
"574",
"17 %" 
],
[
 "SOS",
"1364",
"39 %" 
],
[
 "Disabled Access",
"1135",
"33 %" 
],
[
 "Toilets",
"1168",
"34 %" 
],
[
 "Showers",
"1382",
"40 %" 
],
[
 "Tourist Offices",
"471",
"14 %" 
],
[
 "Children areas",
"451",
"13 %" 
],
[
 "Surf",
"257",
"7 %" 
] 
];
data.addColumn('string','Services');
data.addColumn('string','Number of Beaches');
data.addColumn('string','% of total');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID3bb1cc36441() {
var data = gvisDataTableID3bb1cc36441();
var options = {};
options["allowHtml"] = true;
options["page"] = "enable";

    var chart = new google.visualization.Table(
    document.getElementById('TableID3bb1cc36441')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID3bb1cc36441);
})();
function displayChartTableID3bb1cc36441() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID3bb1cc36441"></script>
 
<!-- divChart -->
  
<div id="TableID3bb1cc36441" 
  style="width: 80%; height: automatic;">
</div>


<br>
*Spain is the top 1 in blue flag award. [Ranking](http://www.blueflag.org/menu/awarded-sites)

--- .class #id 

## Average width and length of the beaches



<!-- BubbleChart generated in R 3.2.0 by googleVis 0.5.8 package -->
<!-- Sun Apr 26 13:26:44 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataBubbleChartID27735b762c0 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Andalucia",
38,
1341,
"Andalucia",
398 
],
[
 "Asturias",
49,
344,
"Asturias",
202 
],
[
 "C. Valenciana",
32,
847,
"C. Valenciana",
328 
],
[
 "Canarias",
28,
359,
"Canarias",
578 
],
[
 "Cantabria",
45,
634,
"Cantabria",
77 
],
[
 "Catalunya",
41,
529,
"Catalunya",
404 
],
[
 "Ceuta",
20,
328,
"Ceuta",
16 
],
[
 "Euskadi",
55,
435,
"Euskadi",
67 
],
[
 "Galicia",
28,
323,
"Galicia",
843 
],
[
 "Illes Balears",
36,
346,
"Illes Balears",
344 
],
[
 "Melilla",
59,
341,
"Melilla",
8 
],
[
 "Murcia",
23,
515,
"Murcia",
198 
] 
];
data.addColumn('string','Region');
data.addColumn('number','Avg.Width');
data.addColumn('number','Avg.Length');
data.addColumn('string','Region.1');
data.addColumn('number','num.beaches');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartBubbleChartID27735b762c0() {
var data = gvisDataBubbleChartID27735b762c0();
var options = {};
options["height"] =    500;
options["width"] =   1000;
options["hAxis"] = {title:'Avg beaches width (m)'};
options["vAxis"] = {title:'Avg beaches length (m)'};

    var chart = new google.visualization.BubbleChart(
    document.getElementById('BubbleChartID27735b762c0')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartBubbleChartID27735b762c0);
})();
function displayChartBubbleChartID27735b762c0() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartBubbleChartID27735b762c0"></script>
 
<!-- divChart -->
  
<div id="BubbleChartID27735b762c0" 
  style="width: 1000; height: 500;">
</div>

<br>
The data is shown by Autonomous Communities. 


--- .class #id 
## Shiny application

The following shiny application is only the first step of this research and the goal 
is to be available of discovering beaches through their equiptments and properties. 
You will only see the filters for:
- Occupation level
- Urbanization level
- Length
- Width
- Vegetation

There are only these filters in the application due to the delivery date of the 
course Developing data product from the [Data Science Specialization](https://www.coursera.org/specialization/jhudatascience/1?utm_medium=catalog)


--- .class #id 
## How to use the shiny application

You will see on the left of the web page the filters for filtering the data. By
default is selected "Low" in Occupation level and "Semiurban" in Urbanization level.
It is because the google map doesn't show the points if there are too many. 

After filtering, you can click on the map's points and see more information about
the beaches. 

<br>
Shiny application: [Beaches Project](https://sergioaguado.shinyapps.io/Beaches_project/)

<br>
I hope that you enjoy this application by discovering nice beaches for going this
summer. 


