---
layout: post
title: FAQs
permalink: /faqs/
index: true
---
<h2>Frequently Asked Questions <i class="fas fa-question-circle" aria-hidden="true"></i></h2>
  <div class="row">
  	<div class="columns">
   	<ul class="accordion" data-accordion data-allow-all-closed="true">
    {% assign sorted = site.faqs | sort: 'order' %}
    {% for faq in sorted %}
    <li class="accordion-item" data-accordion-item>
    <a href="#{{ faq.order }}" class="accordion-title"><b class="blue"><i class="fas fa-chevron-right" aria-hidden="true"></i> {{ faq.title }}</b></a>
    <div class="accordion-content" align="justify" data-tab-content>
									     {{ faq.content }}
						 </div>
    </li>
    {% endfor %}
   </ul>
  </div>
 </div>