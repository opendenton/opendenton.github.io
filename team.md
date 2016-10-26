---
layout: page
date: 2016-02-22T08:35:01-06:00
title: "Our Team"
permalink: /team/
---
<div class="row m-t-3">

	{% for author in site.data.authors %}

	<div class="col-md-4 col-sm-6">
		<div class="politician">
			<figure>
				<img src="https://www.gravatar.com/avatar/{{ author.gravatar }}?s=300" title="{{ author.name }}" class="img-responsive img-thumbnail">
				<figcaption class="poli_img_des">
					{% if author.name %}<h6>{{ author.name }}</h6>{% endif %}
					{% if author.title %}<span>{{ author.title}}</span>{% endif %}
					{% if author.bio %}<p>{{ author.bio }}</p>{% endif %}
				</figcaption>
			</figure>
			<div class="politician_des">
				{% if author.name %}<h6>{{ author.name }}</h6>{% endif %}
				{% if author.title %}<span>{{ author.title}}</span>{% endif %}
				<ul>
					{% if author.facebook %}<li><a href="{{ author.facebook }}"><i class="fa fa-facebook"></i></a></li>{% endif %}
					{% if author.twitter %}<li><a href="{{ author.twitter }}"><i class="fa fa-twitter"></i></a></li>{% endif %}
					{% if author.github %}<li><a href="{{ author.github }}"><i class="fa fa-github"></i></a></li>{% endif %}
					{% if author.email %}<li><a href="mailto:{{ author.email }}"><i class="fa fa-paper-plane"></i></a></li>{% endif %}
				</ul>
			</div>
		</div>
	</div>

	{% endfor %}


</div>