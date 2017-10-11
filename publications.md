---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
    

  - author: "Yingbin Wang, Yiming Li, Daiqin Yang, Zhenzhong Chen"
    title: "A Fast Intra Prediction Algorithm for 360-Degree Equirectangular Panoramic Video"
    month: "December"
    year: "2017"
    address: "St. Petersburg (FL), USA"
    booktitle: "Visual Communications and Image Processing (VCIP)"
    
  - author: "Bin Xu, Xiang Pan, Yan Zhou, Yiming Li, Daiqin Yang, Zhenzhong Chen"
    title: "CNN-Based RateDistortion Modeling for H.265/HEVC"
    month: "December"
    year: "2017"
    address: "St. Petersburg (FL), USA"
    booktitle: "Visual Communications and Image Processing (VCIP)"

  - author: "Yiming Li, Jizheng Xu, Zhenzhong Chen"
    title: "Spherical Domain Rate-Distortion Optimization for 360-Degree Video Coding"
    url: "http://ieeexplore.ieee.org/document/8019492/"
    month: "July"
    year: "2017"
    address: "HongKong, China"
    booktitle: "IEEE International Conference on Multimedia and Expo (ICME)"

  - author: "Yiming Li, Hongyi Liu, Zhenzhong Chen"
    month: "October"
    year: "2016"
    title: "Perceptually lossless Image Coding Based on Foveated-JND and H.265/HEVC"
    url: "http://www.sciencedirect.com/science/article/pii/S1047320316301511"
    booktitle: "Journal of Visual Communication and Image Representation (JVCIR) 40 (2016): 600-610"

  - title: "Recent advances in perceptual H.265/HEVC video coding"
    author: "Zhenzhong Chen, Yiming Li"
    month: "July"
    year: "2015"
    url: "http://ieeexplore.ieee.org/document/7230466/"
    address: "Chengdu, China"
    booktitle: "IEEE China Summit & International Conference on Signal and Information Processing (ChinaSIP)"

  - title: "Perceptually Lossless Image Coding Based on Foveated JND"
    author: "Yiming Li, Hongyi Liu, Zhenzhong Chen"
    month: "August"
    year: "2015"
    url: "http://ieeexplore.ieee.org/document/7300957/"
    address: "San Francisco, CA, USA"
    booktitle: "IEEE International Conference on Information Reuse and Integration (IRI)"

  - title: "Saliency based perceptual HEVC"
    author: "Yiming Li, Weihang Liao, Junming Huang, Da He, Zhenzhong Chen"
    booktitle: " IEEE International Conference on Multimedia and Expo Workshop (ICMEW)"
    address: "Chengdu, China"
    month: "July"
    year: "2014"
    url: "http://ieeexplore.ieee.org/document/6890644/"



---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
    {% if pub.img %}{{pub.img}}.
    {% endif %}
{% endunless %}
{% endfor %}



