---
layout: default
---

<h1 class="post-title">Canadian Data Curation Forum</h1>
The Canadian Association of Research Libraries’ Portage Network in collaboration with McMaster University Library will host a SSHRC-funded Canadian Data Curation Forum at McMaster University in Hamilton from <strong>October 16 to 18, 2019</strong>.  


The goal of the Forum is to establish a national Community of Practice that will catalyze the development/adoption of data curation1 standards, practices, tools, and skills within and across disciplines and institutions. It will bring together library data specialists, research data managers, and discipline and functional experts from a range of institutions and organizations. The Forum will integrate a variety of keynote talks, discussions, and workshops to with the objectives of a) facilitating communication and collaboration around data curation practices and standards, and b) developing skill and training resources.

<h1 class="post-title">News</h1>

<ul class="listing">
{% for post in site.posts %}
  <li class="listing-item">
   <p><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }} | {{ post.date | date: "%B %-d, %Y" }}</a></p>
    <div>
        {{ post.excerpt }}<a class="excerpt" href="{{ site.baseurl }}{{ post.url }}"> Keep reading...</a>
    </div>
  </li>

{% endfor %}
</ul>
