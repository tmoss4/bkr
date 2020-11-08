---
layout: page-fullwidth
header:
   image_fullwidth:
subheadline:
title:  "Educational System"
teaser: 
permalink: "/education/system-exam-results/"
breadcrumb: true
zingchart: true

categories:
    - education
tags:
    - blog
    - content
    - post
    - post format

---
>
In previous years, only half of graduating high school students actually achieve a diploma in any given year. The rest are awarded a 'certificate of attendance,' meaning they went to class, but did not achieve the standard required for graduation.
<br/>- [State of the Nation Report, page 17][3] 

## System

School enrollment is mandatory for children between the ages of 5 and 16. Across the Bahamas there are approximately 169 public schools and 77 private schools. National exams include the Grade Learning Assessment Test (GLAT), Bahamas Junior Certificate (BJC), and Bahamas General Certificate of Secondary Education (BGCSE).

Many primary and secondary schools have Catholic affliations and are under the jurdisction of (or connected to) the [Catholic Board of Education][7].

Tertiary education is primarily available from the [University of The Bahamas][4], however, there are other institutions such as the [National Training Agency][5] and the [Bahamas Technical and Vocational Institute][6].

## Exam Results

Despite many claims, our national results show little progress regardless of which political party is in power. The reasons behind this are discussed in the main <a href="{{ site.url }}{{ site.baseurl }}/education">Education</a> section.

<center>
<a href="http://www.thefirstsay.org/education/immeasurable_progress.php"><img src="{{ site.urlimg }}bgcse-scores.png" alt=""></a>
</center>

Reposted without permission from [TheFirstSay][1].
{: .text-right }

The problem, of course, extends prior to 2004. Ralph Massey authored an interesting paper on [Academic Failure & The Skills Gap][2] in 2006. He notes that, "since this testing system was started in 1993 the results have always been summarized with a single grade, a D+, D, or D-." In the paper, Ralph examines the stark contrast in examination results between the top private school (St. Augustine's College) and the top public school (C.R. Walker). 

Averages have, unfortunately, hidden the depth of the problem. As many Bahamians know historically, private schools like St. Augustine's and Queen's College have typically done much better in national exams than their public school counterparts. The graph below is reproduced from his report and Ralph notes that, "in reality the Bahamas has had a Public School learning problem for several decades and, by talking about the average score for all schools and all subjects, the severity of the problem was not visible to parents and voters." The results were reported this way intentionally, of course, in order to avoid public embarrasment and fool ourselves as far as possible.

<div id="chartDiv"></div>
<center>66% of CR Walker results were below a C grade compared to 15% at St. Augustines</center>

<div class="row">
	<div class="small-6 columns t30">
		<div id="chartDiv2"></div>
	</div><!-- /.medium-3.columns -->

	<div class="small-6 columns t30">
		<div id="chartDiv3"></div>
	</div><!-- /.medium-3.columns -->
</div><!-- /.row -->

<center>These results are for New Providence public schools in 2006 but, as we saw in the first graph, little has changed since then.</center>
<br/>

The State of the Nation Report notes that "The same report quantifies the low results across 2012 GLAT, BJC, and BGCSE exams with ~50% of students scoring below a C in all three sets of tests. The graphs in this section are particularly noteworthy. Here we can see the same trend continues with private schools performing better. More private school students receive grades A-C but the line drops significantly after a grade of C while public schools results for those scores remain high.

The importance of literacy cannot be understated and while some sources report literacy at much higher levels in recent years ([95% in the State of the Nation Report][3]), this has clearly not translated into higher BGCSE English scores. This suggests that something is either wrong with how 'literacy' is being defined and measured, or something wrong with the exam itself. 

Things at the Bahamas Technical and Vocational Institute (BTVI) are not significantly better. "Only one-quarter of the students graduate on time and many take up to five years to complete their programmes." [State of the Nation Report, page 22][3]

<!-- SAC vs CR Walker 2006  Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<script>
var chartData = {
      type: "bar",
      title: {
        text: "2006 BGCSE Results (All Subjects)",
        "font-size":16
      },
      "scale-x": {
       "items-overlap": false,
       label: {
        text: "Letter Grade"
      },
      values: ["A","B","C","D","F"] 
    },
    "scale-y":{
      label: {
        text: "Percentage of All Scores"
      },
      step: 20,
      format: "%v%"
    },
    plot:{
      tooltip:{
        visible : true,
        text: "%t - %v%"
      }
    },
      legend: {
        x: "20%",
        y: "20%"
    },
      series: [
      { 
        values: [4,8,22,24,42],
        backgroundColor:"#2870B1",
        text: "C.R. Walker"
      }, {
        values: [15,23,47,12,3],
        text: "St. Augustines",
        backgroundColor:"#BF0000",
      }
      ]
    };
    zingchart.render({
      id: "chartDiv",
      data: chartData,
      height: 400,
    });
  </script>

<!-- NP Public High BGCSE English and Math Scores Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<script>
  var chartData2 = {
      type: "pie",
      title: {
        text: "BGCSE Results English",
        "font-size": 16,
      },
    "plot":{
    "value-box":{
      "font-size":14,
      "font-weight":"normal",
      "placement":"out",
      "text": "%t - %npv%"
    },
    "tooltip":{
      visible: false
    }
  },
      series: [
      {values: [17],
        backgroundColor:"#7E971D",
        text: "Illiterate"},

      {values: [39],
        backgroundColor:"#2870B1",
        text: "Fail"},

      {values: [44],
        backgroundColor:"#BF0000",
        text: "Pass"},
      ]
    };
    zingchart.render({
      id: "chartDiv2",
      data: chartData2,
      height: 300,
    });
  </script>

<!-- NP Public High BGCSE English and Math Scores Graph -->
<!--Note: Comments using javascript convention (//) will result in build errors-->
<script>
  var chartData3 = {
      type: "pie",
      title: {
        text: "BGCSE Results Math",
        "font-size": 16,
      },
    "plot":{
    "value-box":{
      "font-size":14,
      "font-weight":"normal",
      "placement":"out",
      "text": "%t - %npv%"
    },
    "tooltip":{
      visible: false
    }
  },
      series: [
      {values: [46],
        backgroundColor:"#7E971D",
        text: "Illiterate"},

      {values: [36],
        backgroundColor:"#2870B1",
        text: "Fail"},

      {values: [18],
        backgroundColor:"#BF0000",
        text: "Pass"},
      ]
    };
    zingchart.render({
      id: "chartDiv3",
      data: chartData3,
      height: 300,
    });
  </script>

[1]: http://www.thefirstsay.org/
[2]: http://www.nassauinstitute.org/files/AcademicFailure&SkilsGap3.pdf
[3]: http://www.vision2040bahamas.org/media/uploads/State_of_the_Nation_Summary_Report.pdf
[4]: http://www.ub.edu.bs/
[5]: http://ntabahamas.org/
[6]: http://www.btvi.edu.bs/jhome/
[7]: http://cboe.cec.edu.bs/