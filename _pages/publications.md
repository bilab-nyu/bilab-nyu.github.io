---
title: "biLAB | Publications"
layout: gridlay
excerpt: "biLAB | Publications."
sitemap: false
permalink: /publications/
---


# Publications
## Journal and Submitted Papers

{% for publi in site.data.publist %}
---
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endfor %}
  
## Book Chapter

{% for book in site.data.books %}
---
  {{ book.apa }} <br />

{% endfor %}
  
## Conferences

### 2021

{% for conf in site.data.conf21 %}
---
  {{ conf.conf21 }} <br />

{% endfor %}

### 2020

{% for conf in site.data.conf20 %}
---
  {{ conf.conf20 }} <br />

{% endfor %}

### 2019

{% for conf in site.data.conf19 %}
---
  {{ conf.conf19 }} <br />

{% endfor %}

### 2018

{% for conf in site.data.conf18 %}
---
  {{ conf.conf18 }} <br />

{% endfor %}

### 2017

{% for conf in site.data.conf17 %}
---
  {{ conf.conf17 }} <br />

{% endfor %}

### 2016

{% for conf in site.data.conf16 %}
---
  {{ conf.conf16 }} <br />

{% endfor %}

### 2015

{% for conf in site.data.conf15 %}
---
  {{ conf.conf15 }} <br />

{% endfor %}

### 2014

{% for conf in site.data.conf14 %}
---
  {{ conf.conf14 }} <br />

{% endfor %}

### 2013

{% for conf in site.data.conf13 %}
---
  {{ conf.conf13 }} <br />

{% endfor %}

### 2012

{% for conf in site.data.conf12 %}
---
  {{ conf.conf12 }} <br />

{% endfor %}

### 2010

{% for conf in site.data.conf10 %}
---
  {{ conf.conf10 }} <br />

{% endfor %}

### 2009

{% for conf in site.data.conf09 %}
---
  {{ conf.conf09 }} <br />

{% endfor %}

### 2008

{% for conf in site.data.conf08 %}
---
  {{ conf.conf08 }} <br />

{% endfor %}

### 2007

{% for conf in site.data.conf07 %}
---
  {{ conf.conf07 }} <br />

{% endfor %}

### 2006

{% for conf in site.data.conf06 %}
---
  {{ conf.conf06 }} <br />

{% endfor %}

### 2005

{% for conf in site.data.conf05 %}
---
  {{ conf.conf05 }} <br />

{% endfor %}

### 2004

{% for conf in site.data.conf04 %}
---
  {{ conf.conf04 }} <br />

{% endfor %}

### 2003

{% for conf in site.data.conf03 %}
---
  {{ conf.conf03 }} <br />

{% endfor %}

### 2002

{% for conf in site.data.conf02 %}
---
  {{ conf.conf02 }} <br />

{% endfor %}
  


  