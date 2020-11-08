---
layout: page-fullwidth
header:
   image_fullwidth:
subheadline:
title:  "Corruption"
teaser: 
permalink: "/issues/corruption/"
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
The Bahamas has been judged by the Organization of American States to have substantially implemented the required (anti-corruption*) measures. However, the critical issue is the extent to which actual daily practices of those within the public sector meet or fall short of formal conduct norms. In this regard, concerns have been raised by both domestic and international organizations about the conduct of public officials." [State of the Nation Report, page 38][1]

Cronyism: the appointment of friends and associates to positions of authority, without regard to their qualifications.

*The Bahamas has been a signatory to the 1996 Inter-American Convention Against Corruption since 1998. This Convention sets out public sector conduct norms for the proper fulfilment of public functions by public authorities. The Convention also sets out mechanisms to prevent, criminalise and investigate acts of corruption within the public sector. 

"Additionally, the limited use of strategic and operating plans and performance metrics and the historic absence of integrated and programme-based budgeting can be seen not only as operational challenges but as gaps in reporting to Parliament and ultimately the public. Although the office of the Auditor General and the Public Service Commission add to the capacity of Parliament to hold the government to account, there is a need for the establishment of an Ombudsman office to represent the interests of the public by investigating and addressing complaints of maladministration of public authorities and the strengthening of the Public Accounts Committee to ensure it performs more effectively. Additionally, the enactment of freedom of information legislation will encourage more transparency and government accountability because such legislation grants the public a general right to access records held by public authorities. **Although the Freedom of Information Bill 2015 was released to the public in 2015, its enactment into law remains pending.**" [State of the Nation Report, pages 37-38][1]

"...Based on an incidence of graft index (including expectation of giving a gift in order to receive certain services), The Bahamas’ score at 13.4 ranks high compared to region (6.6) and OECD countries (5.7)." [State of the Nation Report, page 78][1]

<!-- Murder Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<div id="chartDiv"></div>
<script>
	var chartData = {
      type: "bar",
      title: {
        text: "Graft Index (Expectation of Giving a Gift to Receive Certain Services)"
      },
      "scale-x": {
       "items-overlap": false,
       label: {
        text: "Year"
      },
      values: ["Bahamas","Region","OECD Countries"] 
    },
    "scale-y":{
    	label: {
    		text: "Index Score"
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
      	values: [13.4],
      	backgroundColor:"#BF0000",
      	text: "Bahamas"
      }, { 
      	values: [6.6],
      	backgroundColor:"#BF0000",
      	text: "Caribbean Region"
      }, { 
      	values: [5.7],
      	backgroundColor:"#BF0000",
      	text: "OECD Countries"
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