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
  background_image: Working-Space2.jpg
  background_video: Working-Space2.mp4
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
  layout="1"
  block="cta-2"
  section_content_align="left"
  section_image="section-2.jpeg"
  section_overlay="rgba(13, 57, 181, 0.8)"
  section_content_color="light"

%}



{% include blog.html
  grid="1-3"
  gutter="large"
  count="3"
  view_all="/blog/"
    section_title="Uutiset"
  section_subtitle="Lue WhiteWaterin uusimmat kuulumiset"
  section_header_align="center"
%}




{% include cards.html

  block="home-why"
  block_title="false"
  section_size="large"
    grid="1-2"
  gutter="large"
  card_style="default"
  section_background="default"
  section_padding_remove="top"
  section_title="Muutamia töitämme"

  section_header_align="center"
%}

{% include map.html
  latitude="19.419897"
  longitude="-99.164967"
  zoom="12"
  style="silver"
%}


{% else %}


{% endif %}
