---
layout: page-fullwidth
subheadline:
title:  "Unemployment"
meta_title: "BKR - Unemployment"
topic: "BKR"
teaser: ""
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
Youth unemployment is particularly high in the Bahamas with rates sometimes double the national rate.

<!-- Unemployment Graph -->
<!--Chart Placement[2]-->
<div id="chartDiv"></div>
<script>
	var chartData = {
      type: "bar",  // Specify your chart type here.
      title: {
        text: "Unemployment in the Bahamas by Year" // Adds a title to your chart
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
    		text: "Unemployment-rate"
    	},
    	format: "%v%"
    },
    "crosshair-x":{
    	plotLabel:{

    	}
    },
    plot:{
    	tooltip:{
    		visible : false
    	}
    },
      series: [  // Insert your series data here.
      { 
      	values: [7.6, 7.9, 8.7, 14.2,,13.7, 14.0, 15.4, 15.7, 14.8],
      	backgroundColor:"#0011AB",
      	text: "Unemployment-rate"
      }
      ]
  };
    zingchart.render({ // Render Method[3]
    	id: "chartDiv",
    	data: chartData,
    	height: 400,
    });
</script>

Source: [Trading Economics][1]
{: .text-right }

[1]: http://www.tradingeconomics.com/bahamas/unemployment-rate