---
layout: page-fullwidth
header:
   image_fullwidth: "bpano.jpeg"
subheadline:
title:  "Gross Domestic Product (GDP)"
teaser: 
permalink: "/issues/gdp/"
breadcrumb: true
zingchart: true

categories:
    - issues
tags:
    - blog
    - content
    - post
    - post format

---
>
Tourism, the country’s main industry, employs half the labour force and directly and indirectly accounts for about 60% of the Gross Domestic Product (GDP). The financial services industry employs 10% of the population and generates 10-15% of GDP.

The Bahamas is among the richest Caribbean nations. Our proximity to the US and use as an offshore financial outlet have led to an amazing level of wealth. When looking at raw GDP, it is easy to tell a story of recovery from the 2008 financial crisis and see a trend of growth. However, this would be a gross oversimplification. To build a more complete picture, we must also examine GDP growth rate, GDP per capita, gross domestic savings, and foreign direct investment at the least.

<div id="chartDiv3"></div>
Source [Trading Economics][4]
{: .text-right }

While these are certainly high numbers, the graph below shows that when divided by the population, we have not seen substantial recovery from the economic crisis. Still, the Bahamas is significantly above the [Caribbean regional average][5], nearly double according to the World Bank.

<div id="chartDiv2"></div>
Source [Trading Economics][2]
{: .text-right }

GDP growth rate is another important factor and here we can see most clearly the effects of the financial crisis. As a small island developing state (SIDS), economic growth has always been a challenge. 

<div id="chartDiv"></div>
Source [Trading Economics][3]
{: .text-right }

Let's go back even further and compare to US growth in the graph below.

<h5><center>The Bahamas and the United States GDP Growth for 1991-2014</center></h5>
<center>
<a href="http://www.vision2040bahamas.org/media/uploads/State_of_the_Nation_Summary_Report.pdf"><img src="{{ site.urlimg }}bahamas-us-gdp-growth.png" alt=""></a>
</center>
<center>State of the Nation Report, page 61</center>

<br/>
The US is a global power and international markets rise and fall as the US market does. As an economic partner, vacation destination, study abroad location, and geographical neighbor, the Bahamas' success is tied closely to the US'. 

<h5><center>Gross Domestic Savings and Foreign Direct Investment from 1996-2014 (% of GDP)</center></h5>
<center>
<a href="http://www.vision2040bahamas.org/media/uploads/State_of_the_Nation_Summary_Report.pdf"><img src="{{ site.urlimg }}gds-fdi.png" alt=""></a>
</center>
<center>State of the Nation Report, page 61</center>

<br/>
"Foreign Direct Investment is key to our economy; yet our ability to convert these investments into greater national wealth lags compared to others in the region." - [State of the Nation Report, pages 62][1]

Losses due to damage from extreme events affect the country’s financial stability. Hurricane Sandy in 2012 was a relatively low intensity hurricane that still had a total economic cost of $702.8 million, approximately 9% of the GDP. - [State of the Nation Report, pages 56][1]

National debt...

<!-- GDP Growth Rate Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<script>
	var chartData = {
      type: "bar",
      title: {
        text: "Bahamas GDP Annual Growth Rate",
        "font-size": 20
      },
      "scale-x": {
       "items-overlap": false,
       label: {
        text: "Year"
      },
      values: [2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015] 
    },
    "scale-y":{
    	label: {
    		text: "Percentage Growth Rate"
    	},
    	"min-value": -5,
    	"max-value": 5,
    	step: 1,
    	format: "%v%"
    },
    "crosshair-x":{
    	plotLabel:{
			"text": "%t - %v%"
    	}
    },
    plot:{
    	tooltip:{
    		visible : false
    	}
    },
      series: [
      { 
      	values: [2.5, 1.4, -2.3, -4.2, 1, 1.7, 1.8, 1.9, 1, 1.2],
      	backgroundColor:"#0011AB",
      	text: "GDP Growth Rate"
      }
      ]
    };
    zingchart.render({
    	id: "chartDiv",
    	data: chartData,
    	height: 400,
    });
  </script>

<!-- GDP Per Capita Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<script>
	var chartData2 = {
      type: "bar",
      title: {
        text: "Bahamas GDP Per Capita",
        "font-size": 20
      },
      "scale-x": {
       "items-overlap": false,
       label: {
        text: "Year"
      },
      values: [2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015] 
    },
    "scale-y":{
    	label: {
    		text: "USD"
    	},
    	"min-value": 20000,
    	short: true
    },
    "crosshair-x":{
    	plotLabel:{
			"text": "%t - %v"
    	}
    },
    plot:{
    	tooltip:{
    		visible : false
    	}
    },
      series: [
      { 
      	values: [24430.74, 24316.49, 23320.22, 21956.46, 21920.52, 21701.17, 21844.19, 21533.67, 21457.87, 21441.84],
      	backgroundColor:"#0011AB",
      	text: "GDP Per Capita",
      	"thousands-separator":","
      }
      ]
    };
    zingchart.render({
    	id: "chartDiv2",
    	data: chartData2,
    	height: 400,
    });
  </script>

<!-- GDP  -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<script>
	var chartData3 = {
      type: "bar",
      title: {
        text: "Bahamas GDP",
        "font-size": 20
      },
      "scale-x": {
       "items-overlap": false,
       label: {
        text: "Year"
      },
      values: [2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015] 
    },
    "scale-y":{
    	label: {
    		text: "USD Billion"
    	},
    	"min-value": 7800000000,
    	short: true
    },
    "crosshair-x":{
    	plotLabel:{
			"text": "%t - %v"
    	}
    },
    plot:{
    	tooltip:{
    		visible : false
    	}
    },
      series: [
      { 
      	values: [7970000000, 8320000000, 8250000000, 7820000000, 7910000000, 7890000000, 7890000000, 8230000000, 8430000000, 8510000000, 8880000000],
      	backgroundColor:"#0011AB",
      	text: "GDP",
      	short: true
      }
      ]
    };
    zingchart.render({
    	id: "chartDiv3",
    	data: chartData3,
    	height: 400,
    });
  </script>

[1]: http://www.vision2040bahamas.org/media/uploads/State_of_the_Nation_Summary_Report.pdf
[2]: http://www.tradingeconomics.com/bahamas/gdp-growth-annual
[3]: http://www.tradingeconomics.com/bahamas/gdp-per-capita
[4]: http://www.tradingeconomics.com/bahamas/gdp
[5]: http://en.wikipedia.org/wiki/List_of_Latin_American_and_Caribbean_countries_by_GDP_(PPP)#cite_note-1
