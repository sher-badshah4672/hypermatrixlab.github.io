---
layout: about
title: Home
permalink: /
subtitle:

profile:
  align: right
  image: mainlp-logo-500.png
  image_circular: false
  address:

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

groups: [staff]
staff:
  title: Research Staff
  people:
    - name: Barbara Plank
      description: Prof. Dr. and Chair for AI and Computational Linguistics, Head of MaiNLP and Co-director CIS
      website: https://bplank.github.io/
      picture: barbara.jpg
    - name: Diego Frassinelli
      description: Dr., Lecturer
      website: https://www.cis.uni-muenchen.de/personen/mitarbeiter/frassinelli/index.html
      picture: mainlp-logo-500.png
    - name: Michael A. Hedderich
      description: Junior Research Group Leader
      website: https://www.michael-hedderich.de/
      picture: michael.jpg
    - name: Silvia Casola
      description: Postdoc (2024–)
      website: https://scholar.google.it/citations?user=h6Nw1QIAAAAJ
      picture: mainlp-logo-500.png
    - name: Yang Janet Liu
      description: Postdoc (2024–)
      website: https://janetlauyeung.github.io/
      picture: janet.png
    - name: Siyao (Logan) Peng
      description: Postdoc (2023–)
      website: https://logan-siyao-peng.github.io/
      picture: logan.jpeg
    - name: Robert Litschko
      description: Postdoc (2022–)
      website: https://rlitschk.github.io/
      picture: robert.png
    - name: Andreas Säuberli
      description: PhD student (2024–)
      website: https://saeub.github.io/
      picture: mainlp-logo-500.png
    - name: Felicia Körner
      description: ELLIS PhD student (2024–)
      website: https://koernerfelicia.github.io/
      picture: felicia.JPG
    - name: Florian Eichin
      description: PhD student (2024–)
      website: https://florian-eichin.com/
      picture: florian.png
    - name: Soh-Eun (Ryan) Shim
      description: PhD student (2024–)
      website: https://www.cis.lmu.de/personen/mitarbeiter/soheunshim/index.html
      picture: mainlp-logo-500.png
    - name: Shijia Zhou
      description: PhD student (2024–)
      website: https://scholar.google.com/citations?user=Byl83QwAAAAJ
      picture: shijia.jpg
    - name: Beiduo Chen
      description: ELLIS PhD student (2024–)
      website: https://mckysse.github.io/
      picture: beiduo.jpg
    - name: Philipp Mondorf
      description: PhD student (2023–)
      website: https://pmmon.github.io/
      picture: philipp.jpg
    - name: Xinpeng Wang
      description: PhD student (2022–)
      website: https://xinpeng-wang.github.io/
      picture: xinpeng.jpg
    - name: Verena Blaschke
      description: PhD student (2022–)
      website: https://verenablaschke.github.io/
      picture: verena.png
    - name: Elena Senger
      description: External PhD student (2023–), Fraunhofer IMW
      website: https://elenasenger.netlify.app/
      picture: elena.jpg

---

Welcome!
We are the Munich AI & NLP (MaiNLP, pronounced "myNLP") research lab at the [Center for Information and Language Processing (CIS)](https://www.cis.lmu.de/), LMU Munich, directed by [Prof. Dr. Barbara Plank](https://bplank.github.io/).
We carry out research in Natural Language Processing, an interdisciplinary subdiscipline of Artificial Intelligence at the interface of computer science, linguistics and cognitive science.
In broad terms, our aim is human-facing NLP: to make NLP models more robust and inclusive, so that they can deal better with underlying shifts in data due to language variation, are fairer and embrace human label variation.

<div class="projects">
  <h2 class="category">News</h2>
  <ul>
    <li>August 14, 2024: Barbara gave a <a href="https://2024.aclweb.org/program/keynotes/">keynote at ACL 2024</a> in Bangkok this year</li>
    <li>July 10, 2024: We co-organized a panel on <a href="https://mainlp.github.io/iclave12/">embracing variability in natural language processing</a> at ICLaVE|12</li>
    <li>July 5, 2024: Max successfully defended his PhD thesis. Congratulations!</li>
    <li>July 1, 2024: Elisa successfully defended her PhD thesis. Congratulations!</li>
    <li>May 13, 2024: On-site <a href="/events/#2024-05-13-matthias-orlikowski">talk</a> by Matthias Orlikowski (Bielefeld University)</li>
    <li>May 6, 2024: On-site <a href="/events/#2024-05-06-russa-biwas">talk</a> by Dr. Russa Biwas (Hasso-Plattner Institute, Potsdam)</li>
    <li>April 30, 2024: Our new <a href="https://dialect-erc.github.io">DIALECT project</a> webpage is online</li>
    <li>April 8, 2024: On-site <a href="/events/#2024-04-08-hyewon-jang">talk</a> by Hyewon Jang (University of Konstanz)</li>
    <li>March 22, 2024: Interested in Uncertainty and NLP? We are part of the <a href="https://uncertainlp.github.io/">First Workshop on Uncertainty-aware NLP @ EACL 2024</a></li>
    <li>March 7, 2024: Mike successfully defended his PhD thesis. Congratulations!</li>
    <li>January 24, 2024: On-site <a href="/events/#2024-01-24-rob-van-der-goot">talk</a> by Dr. Rob van der Goot (IT University of Copenhagen)</li>
  </ul>

To <a href="/events-archive/">earlier events</a> at MaiNLP.

{%- for group in page.groups -%}

  <h2 class="category">{{page.[group].title}}</h2>
    <div class="grid">
      {%- for person in page.[group].people -%}
          <article class="grid-item card">
            {% if person.picture -%}
              <img class="avatar" src="/assets/img/{{person.picture}}" alt="Portrait ({{person.name}})" width="auto" height="auto">
            {%- else -%}
              <img class="avatar" src="/assets/img/mainlp-logo-500.png" alt="Portrait ({{person.name}})" width="auto" height="auto">
            {%- endif -%}
          <div class="card-body">
            <!-- <h2 class="card-title">{{person.name}}</h2> -->
            <h2 class="card-title">
              {% if person.website -%}
                <a href="{{person.website}}">{{person.name}}</a>
              {%- else -%}
                {{person.name}}
              {%- endif -%}
            </h2>
            <div class="card-text">
              {{person.description}}
            </div>
            </div>
          </article>
      {%- endfor -%}
    </div>
  {%- endfor -%}

  <h2 class="category">You?</h2>
  Join us! <a href="/jobs">→Open positions</a>

  <h2 class="category">MaiNLP resources and code</h2>
  You can find resources (data, code, repositories) released by MaiNLP lab members <a href="https://github.com/mainlp/">on our github page</a> and <a href="https://huggingface.co/mainlp">on our huggingface page</a>

  <h2 class="category">Organizations</h2>
  Our research is supported by:
  <ul>
    <li><a href="https://erc.europa.eu/homepage">European Research Council (ERC)</a> project <a href="https://mainlp.github.io/projects/#ongoingproj">DIALECT</a></li>
    <li><a href="https://dff.dk/en">Danmarks Frie Forskningsfond (DFF)</a>, Sapere Aude Research Leader grant</li>
    <li><a href="https://www.bayern.de/politik/hightech-agenda/">Bayerische Staatsregierung HTA</a></li>
    <li><a href="https://mcml.ai/">Munich Center for Machine Learning (MCML)</a></li>
    <li><a href="https://www.bidt.digital/">Bayerisches Forschungsinstitut für Digitale Transformation (bidt)</a></li>
  </ul>

We are also part of:

  <ul>
    <li><a href="https://ellis.eu/programs/natural-language-processing">ELLIS Europe NLP Program</a></li>
    <li><a href="https://www.ellismunich.ai/">ELLIS Unit Munich</a></li>
  </ul>

 <!-- TODO <img src="MCML_Logo.jpg" alt="MCML logo"/> -->

  <h2 class="category">Find us</h2>
  We are located at Akademiestraße 7, 80799 Munich, Germany (<a href="https://mainlp.github.io/contact/">→ directions</a>).<br/>

<a href="https://github.com/mainlp"><i class="fab fa-github"></i> MaiNLP</a><br/>
<a href="https://twitter.com/MaiNLPlab"><i class="fab fa-twitter"></i> MaiNLPlab</a><br/>
<a href="https://twitter.com/CisLMU"><i class="fab fa-twitter"></i> CisLMU</a>

</div>
