---
layout: page-fullwidth
header:
   image_fullwidth: "bpano.jpeg"
subheadline:
title:  "Unemployment"
teaser: 
permalink: "/issues/unemployment/"
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
A high percentage of the unemployed have not completed high school which makes them particularly vulnerable. Youth unemployment is very high at around 30%. While having a young, diverse workforce is valuable, high levels of unemployment among the youth can lead to a reduction in social cohesion, limited future employability and loss of skills. Further, as young people remain out of work, the long term earning potential and productivity of this segment of the population diminishes as they lose opportunities to develop additional cognitive and soft skills, gain experience and showcase their creativity. 
<br/>-State of the Nation, page xx

Generally, a healthy employment rate is 4-6%.

Recent unemployment levels across the country stand at 14.8%. The Bahamas was certainly hit hard by the 2008 financial crisis when the unemployment level was still relatively high at 8%.

Young people have been disproportionally affected as youth unemployment is a stark 30%. The State of the Nation Report notes that youth unemployment may be associated with lower levels of well-being in the society, increased mental and behavioural problems, higher incidents of drug and alcohol usage and other high risk activities. The connections between high unemployment levels and crime are well researched and documented.

<div id="chartDiv"></div>
<br/>
Source: [Trading Economics][2] and [International Monetary Fund][4]
{: .text-right }

"Beyond the tag line of youth unemployment is a greater story of lost productivity and deterioration in the health of the Bahamian economy due to lower output, reduced consumption, reduced investment and increased social spending. The low growth rates seen in The Bahamas suggest that it is unlikely that the current industries could grow sufficiently fast to absorb those currently unemployed and the new members entering the workforce yearly. New industries and innovative solutions to increase opportunities will have to be developed. The Bahamas will be facing an increasingly aging population in 2040. With such a high level of its productive workforce out of employment, the country is ill prepared to achieve the level of development to support the changing demographic." [State of the Nation Report, page 26][1]

<!-- Unemployment Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<script>
	var chartData = {
      type: "bar",
      title: {
        text: "Unemployment in the Bahamas by Year"
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
      	values: [7.6, 7.9, 8.7, 14.2, 15.1, 13.7, 14.0, 15.4, 15.7, 14.8],
      	backgroundColor:"#0011AB",
      	text: "Unemployment-rate"
      }
      ]
  };
    zingchart.render({
    	id: "chartDiv",
    	data: chartData,
    	height: 400,
    });
</script>

Ralph Massey authored an interesting paper on [Academic Failure & The Skills Gap][3] in 2006.

[1]: http://www.vision2040bahamas.org/media/uploads/State_of_the_Nation_Summary_Report.pdf
[2]: http://www.tradingeconomics.com/bahamas/unemployment-rate
[3]: http://www.nassauinstitute.org/files/AcademicFailure&SkilsGap3.pdf
[4]: http://www.indexmundi.com/the_bahamas/unemployment_rate.html