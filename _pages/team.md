---
title: "Research Group | biLAB"
layout: gridlay
excerpt: "Research Group biLAB"
sitemap: false
permalink: /team/
---

# Our Lab

<!-- The Building Informatics and Visualization Lab (biLAB) is part of the [Department of Civil and Urban Engineering](https://engineering.nyu.edu/academics/departments/civil-and-urban-engineering) at the [NYU Tandon School of Engineering](https://engineering.nyu.edu/). It focuses on understanding the operational challenges associated with construction and operation of facilities and infrastructure systems in urban settings.

The research team works on information modeling and visualization to quantify the impact of architecture on human experience in the built environment, understand and improve the behaviors of existing/new facilities and civil infrastructure systems for next generation construction, maintenance, and operations. The research team takes advantage of advancements in technology in information modeling and visualization to integrate and provide information that engineers, owners, and facility operators need, at the right level of detail and visual form.

They work on developing information repositories and visualization platforms to better integrate the data captured from sensors and the context under which they operate to get a holistic view of the monitored system/infrastructure for better maintenance and operation.

# Our Team

<img src="/images/semiha2.jpg" width="30%"/>

Dr. Semiha Ergan is a faculty at NYU Tandon School of Engineering, Department of Civil and Urban Engineering with a courtesy appointment at NYU Department of Computer Science and Engineering. She is also an associated faculty member at Center for Urban Science and Progress (CUSP). Prior to joining NYU, she was a research faculty at Carnegie Mellon University, where she also received a Ph.D. in civil engineering.

Her current research interests include IT to support design, construction and operations of civil infrastructure systems, studying urban challenges for AEC/FM, building informatics for efficient and healthier buildings, quantification of human experience in the built environment, and infrastructure information modeling and visualization.

[Prof. Ergan's NYU profile](https://engineering.nyu.edu/faculty/semiha-ergan)

[Prof. Ergan on Google Scholar](https://scholar.google.com/citations?user=WYwmI0wAAAAJ&hl=en)

[Prof. Ergan on ResearchGate](https://www.researchgate.net/profile/Semiha_Ergan)

Please check [Job Openings page](/jobopening) for openings in the research group. -->

### Join Us!

<!-- Positions are available at [PhD](/downloads/Flier-PhD-Ergan_Oct15.pdf) and [PostDoc](/downloads/Flier-Postdoc-Darpa-Ergan.pdf) levels in BiLAB. Please contact Prof. Ergan for details.   -->

Positions are available at PhD levels in BiLAB. Please contact Prof. Ergan for details.  

<img src="/images/IMG-8017.jpg" width="65%"/>

<!-- Jump to [PhD Student](#phd-student), [Master and Bachelor students](#master-and-bachelor-students), [High school students hosted](#high-school-students-hosted), and [Alumni](#alumni). -->

[PhD Students](#phd-student)

<br>

## PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
<h4>{{ member.name }}</h4>
<i>{{ member.info }}<br>email: <{{ member.email }}></i>
<ul style="overflow: hidden">
<p> {{ member.desc }} </p>
</ul>
Research project: {{ member.prj }}
</div>

{% endfor %}
<br>
<br>

## Master and Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br>

## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> {{ member.info }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br>

## Former visitors, BSc/MSc students
<div class="row">
<h4>Visitors</h4>
  {% assign num_students = site.data.alumni_visitors | size %}
  {% assign col_class = 'col-lg-' | append: 12 | divided_by: num_students %}
  {% for member in site.data.alumni_visitors %}
<div class="{{ col_class }} col-sm-3" style="background-color: #f2f2f2; margin: 5px;">
  {{ member.name }}
</div>
  {% endfor %}
</div>

<div class="row">
<h4>Master students</h4>
  {% assign num_students = site.data.alumni_msc | size %}
  {% assign col_class = 'col-lg-' | append: 12 | divided_by: num_students %}
  {% for member in site.data.alumni_msc %}
<div class="{{ col_class }} col-sm-3" style="background-color: #f2f2f2; margin: 5px;">
  {{ member.name }}
</div>
  {% endfor %}
</div>

<div class="row">
<h4>Bachelor students</h4>
  {% assign num_students = site.data.alumni_bsc | size %}
  {% assign col_class = 'col-lg-' | append: 12 | divided_by: num_students %}
  {% for member in site.data.alumni_bsc %}
<div class="{{ col_class }} col-sm-3" style="background-color: #f2f2f2; margin: 5px;">
  {{ member.name }}
</div>
  {% endfor %}
</div>

<br>

## High school students hosted
Summer 2023:  
Samira Maria, <b>Brooklyn Technical High School</b>  
Daisy Sherpa, <b>Forest Hills High School</b>  

Summer 2022:  
Sam Karmarkar, <b>Brooklyn Technical High School</b>  
Motunrayo Owoborode, <b>Young Women's Leadership School of Queens</b>  

Summer 2021:  
Brandon Knox, <b>Peddie School</b>  
Sandy Yuan, <b>Brooklyn Technical High School</b>  

Summer 2020:  
David Ugo-Omernukwa, <b>Bronx High School of Science</b>  
Nyah Smith, <b>Computer Science High School</b>  
  
Summer 2019:  
InesVillegas Costa, <b>Bard High School Early College</b>  
Lauren Pehlivanian, <b>Stuyvesant High School</b>  
  
Summer 2018:  
Tina Wong, <b>Stuyvesant High School</b>  
Daniel Gomez, <b>Stuyvesant High School</b>  
  
Summer 2017:  
Connie Tsang, <b>Hunter College High School</b>  
Jason Cheung, <b>Stuyvesant High School</b>  
  
Summer 2016:  
Danny Dirusso, <b>Dobbs Ferry School District</b>  
<br><br>
