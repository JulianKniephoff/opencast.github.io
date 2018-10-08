---
title: Opencast Community Meetings
---

{% include community_menu.html %}

# Upcoming Events
Here are the conferences and workshops organized by the Opencast community and/or with participation by / relevance for the Opencast community.

{% for post in site.posts %}
{% if post.tags contains "upcoming" %}

{% include box-start.html 
  backgroundcolor=site.data.colors.bluebox 
%}
{% if post.image %}
<img class="fullsizebox-image" src="{{ post.image }}" style="float:right; width:40%;"/>
{% endif %}
<div>
  <h2><a href="{{ post.url | remove_first:'/' }}">{{ post.title }}</a></h2>
    <p><b>{{ post.description }}</b></p>
    <p>{{ post.excerpt }}</p>
  <a href="{{ post.url | remove_first:'/' }}">Read more...</a>
</div>
{% include box-end.html %}

{% endif %}
{% endfor %}

---

# Past Events

{% for post in site.posts %}
{% if post.tags contains "past" %}

{% include box-start.html 
  backgroundcolor=site.data.colors.box 
%}
{% if post.image %}
<img class="fullsizebox-image" src="{{ post.image }}" style="float:left; width:40%;"/>
{% endif %}
<div>
  <h2><a href="{{ post.url | remove_first:'/' }}">{{ post.title }}</a></h2>
    <p>{{ post.description }}</p>
    <p>{{ post.excerpt }}</p>
  <a href="{{ post.url | remove_first:'/' }}">Read more...</a>
</div>
{% include box-end.html %}

{% endif %}
{% endfor %}

{% include fullsizebox.html
title="2018 Opencast summit"
description="The website has recording of most of the sessions of this years conference.
*Thanks to Austria’s Academic Moodle Cooperation for hosting the 2018 Opencast Summit at the University of Vienna.*"
image="assets/img/opencast2018wien.jpg"
align="left"
imagewidth="40%"
linktext="Watch the Vienna Conference Recordings..."
linkurl="http://opencast2018.univie.ac.at/programme-and-recordings/"
%}

{% include fullsizebox.html
title="Conferences and Workshops"
description="There is one major annual meeting, the Opencast Summit. While this used to be an unconference with an open agenda, we are trying to mix planned sessions with open slots these days, based on feedback we got from the community. Usually, there will be a call for participation to the community with a selection of presentations submitted (if necessary) so that a programme is set a couple of weeks before the event. To maintain the \"unconference style\" there will be empty slots for ad hoc sessions or open discussions. Besides the presentation slot(s) we usually organize a vendor showcase for the latest capture agent technology and service provider offerings.

Plus, there are regional Opencast meetings. The German-speaking community for example meets once or twice a year for a workshop.

Last but not least, there is the annual Open Apereo Conference, with members of the Opencast Community joining and – ideally – presenting or organizing seminars and workshops to inform the larger Apereo community about Opencast."
image="assets/img/opencast-summit-2017.jpg"
align="left"
imagewidth="40%"
backgroundcolor=site.data.colors.box
%}


{% include fullsizebox.html
title="Conference Recordings"
description="There are recordings from the annual Opencast Summit since 2012 in the [video archive of the ETH Zürich](https://www.video.ethz.ch/events/opencast.html). You can find many interesting talks on the development of Opencast, user-stories from adopting institutions and many other topics here."
image="assets/img/recording.jpg"
align="left"
linktext="Watch the Conference Recordings..."
linkurl="https://www.video.ethz.ch/events/opencast.html"
imagewidth="40%"
%}

---

# Frequent Meetings

{% include webmeetings.html %}

# Community Calendar

<iframe src="https://calendar.google.com/calendar/embed?title=Opencast%20Community%20Calendar%20(GMT)&amp;height=600&amp;wkst=2&amp;bgcolor=%23FFFFFF&amp;src=opencast.org_tje2fm34ernnbm0f9saiogp8g0%40group.calendar.google.com&amp;color=%23B1440E&amp;ctz=UTC" style="border-width:0" width="800" height="600" frameborder="0" scrolling="no"></iframe>
