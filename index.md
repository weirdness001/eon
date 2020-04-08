---
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 1-1 # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: Working-Space.jpg
  background_video: Working-Space.mp4
#  background_overlay: "linear-gradient(to left top,rgba(218, 91, 197, 0.8) 0%,rgba(151, 27, 191, 0.8) 30%,rgba(2, 8, 212, 0.8) 80%)"
  color: light
  heading_size: medium
  height: full
  parallax: true
  container: small
  content:
    block: header-home
---

[comment]: # (This actually is the most platform independent comment)



{% if site.template == 'base' %}

{% include cta.html
  section_size="large"
  layout="2"
  block="cta-2"
  section_content_align="center"
  section_image="section-2.jpeg"
  section_overlay="rgba(13, 57, 181, 0.8)"

%}

{% include cards.html
  block="card-media"
  section_title="Palvelut"
  section_header_align="center"
  media="top"
  section_size="large"
  section_padding_remove="top"
  section_container="expand"
  section_background="default"
  card_style="default"
  section_content_align="center"
%}



  {% include cards.html
    block="home-why"
    section_title="Töitämme"
    section_header_align="center"
    section_size="large"
    section_background="muted"
    grid="1-3"
    gutter="large"
  %}

  {% include cta.html
    section_size="large"
    section_image="section-2.jpeg"
    section_overlay="rgba(13, 57, 181, 0.8)"
    section_content_color="light"
    layout="3"
    block="cta-6"
  %}


{% else %}


{% endif %}
