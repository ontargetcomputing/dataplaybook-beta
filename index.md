---
layout: default
title: Home
---
![California Health and Human Services Agency Data Playbook - 3rd Edition]({{ site.baseurl }}/assets/images/00_figure01.png "California Health and Human Services Agency Data Playbook - 3rd Edition")
## Data changes everything

With over 33,000 employees, we at CHHS make up the largest agency under California’s executive branch. Our 13 departments collectively have access to an unprecedented amount of data -- it is our mission to use this data to improve the programs and services we deliver to our clients, amplify the impact of the data reports we create, and to create an organizational culture that is focused on data-driven decision making.  

## What’s inside

This playbook is intended to help you with your data project from start to finish. Every member of CHHS -- from the data novice to the data expert -- will find something useful here, whether it’s learning how to analyze a dataset for the first time or refining your knowledge of advanced data visualization. 

### Inside, you will find **four chapters**:

| 1. **[Planning]({{ site.baseurl }}/plan/)** Your Data Project |
| - Setting goals and strategy<br />- What data you will need<br />- Identifying your Data Sources |
| 2. **[Analyzing]({{ site.baseurl }}/analyze/)** Your Data |
|- Cleaning and De-Identifying Your Dataset<br />- Learning Resources<br />- Review: Facts, Stats and Trends |
| 3. **[Communicating]({{ site.baseurl }}/communicate/)** Your Results |
|- Crafting your Data Narrative<br />- Designing Effective Visualizations<br />- Sharing your Findings with Others |
| 4. **[Concluding]({{ site.baseurl }}/maintain/)** Your Project |
|- Product lifecycle & User Feedback<br />- Product Design Strategies |

Additionally, we’ve created a [Resource Library]({{ site.baseurl }}/resource_library/) with a quick summary of all public data sources, skill building and training resources, and useful data analysis tools and software included in the playbook. 

## Our goals for this playbook
This playbook is a living, breathing document that will change and adapt based on our collective experiences. We highly encourage you to [contribute]({{ site.baseurl }}/resource_library/) to the resource library or share your data story -- collaboration will be essential to shaping our organizational culture. It is our hope that each user of this playbook leaves feeling more empowered by the skills they’ve gained and inspired to bring about meaningful change. 


If you need help accessing any of the materials in the Playbook, please contact <dataplaybook@chhs.ca.gov>.

<!-- Pagination -->
<div class="pagination">
  <span class="pagination-item older">&laquo; Prev</span>
  <a class="pagination-item newer" href="{{ site.baseurl }}/plan">Next &raquo;</a>
</div>


<div id="printedpages">
  {% assign pages_list = site.pages %}
  {% for node in pages_list %}
    {% if node.printable == true %}  
      {% capture to_include %}{% include_relative {{node.path | prepend: 'includes/'}} %}{% endcapture %}
      {{ to_include | markdownify }}
    {% endif %}
  {% endfor %}
</div>
