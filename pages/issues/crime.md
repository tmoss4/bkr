---
layout: page-fullwidth
header:
   image_fullwidth: "bpano.jpeg"
subheadline:
title:  "Crime"
teaser: 
permalink: "/issues/crime/"
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
Deteriorating economic conditions and rising unemployment have contributed to the gravely intensified incidents of crime, in particular violent crime, in The Bahamas. In addition to its devastating social impact on communities, rising crime levels constitute a critical threat to the economy, domestic and foreign sectors. It is particularly harmful to tourism, the economy’s principal driver, which is influenced by even the perception of crime. 
<br/>- [State of the Nation Report, page 77][1]

Conviction rates are low and there have been reports of "inadequate institutional capacity".  [State of the Nation Report, page 35][1] 

"The U.S. State Department gave The Bahamas a crime rating of 'critical.' While not a warning, Canada reminded its travelers to 'exercise a high degree of caution due to high rates of crime, especially in Nassau'. One reason attributed to the high crime rates is the delay in administering justice..." [State of the Nation Report, page 39][1]

These kind of travel warnings have become commonplace and many visitors have been vocal about violent incidents and poor service they have received. This issue has gone largely unaddressed.

The United States Department of State heads the Overseas Security Advisory Council (OSAC) which releases annual reports on crime in the Bahamas. You can find the latest report [here][2]. Reports go back until 2012.

[2]: http://www.osac.gov/pages/ContentReportDetails.aspx?cid=19192

<!-- Murder Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<div id="chartDiv"></div>
<script>
	var chartData = {
      type: "bar",
      title: {
        text: "Murders in the Bahamas by Year"
      },
      "scale-x": {
       "items-overlap": false,
       label: {
        text: "Year"
      },
      values: [2000, 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016] 
    },
    "scale-y":{
    	label: {
    		text: "Murder Count"
    	},
    	step: 20
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
      series: [
      { 
      	values: [73, 43, 52, 50, 44, 50, 60, 78, 72, 87, 94, 127, 111, 119, 122, 149, 111],
      	backgroundColor:"#BF0000",
      	text: "Murders"
      }
      ]
    };
    zingchart.render({
    	id: "chartDiv",
    	data: chartData,
    	height: 400,
    });
  </script>

  [1]: http://www.vision2040bahamas.org/media/uploads/State_of_the_Nation_Summary_Report.pdf