---
layout: startpage
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
header: no
---


<div class="page__wrap">

  <section class="hero row row__wrap">
    <div class="columns">
      <h1 class="hero__header">
        <span class="hero__header--name">eGo<sup>n</sup></span>
        <span class="hero__header--text">Open and cross-sectoral planning of transmission and distribution grids</span>
      </h1>
    </div>
    <div class="hero__left large-7 columns">
      <p class="hero__subheader">
        Driven by the expansion of renewable generation capacity and the progressing electrification of other energy sectors, the electrical grid increasingly faces new challenges: fluctuating supply of renewable energy and simultaneously a changing demand pattern caused by sector coupling. However, the integration of non-electric sectors such as gas, heat and e-mobility enables more flexibility options. 
        This project aims to investigate the effects of sector coupling on the electrical grid and the benefits of new flexibility options. Like the previous project <a href="https://openegoproject.wordpress.com" title="open_eGo">open_eGo</a>, this work will follow the open-source and open-data principles.
      </p>
      <div class="hero__btn">
        <a href="/tools_data/" class="button hero__cta">See our tools</a>
      </div>
    </div>
    <div class="hero__right large-5 columns hero__img">
      <img src="images/HP_hero_img_v3_for_web.svg" alt="Gas, heat and e-mobility are coupled on the electrical grid. Data come from the OpenEnergyPlatform">
    </div>
  </section>

  <section class="tasks row row__wrap">
    <div class="small-12 columns tasks__header">
      <h2>Our tasks</h2>
    </div>
    <div class="small-12 columns">
      <div class="tasks__row row">
        <div class="tasks__item medium-6 columns">
          <div class="tasks__item-text">
            <h3 class="tasks__item-title">Sector Coupling</h3>
            We want to identify the opportunities and potentials, but also challenges of progressing sector coupling. We also want to optimize the modelled energy system with regard to the overall costs.
          </div>
        </div>
        <div class="tasks__item medium-6 columns">
          <div class="tasks__item-text">
            <h3 class="tasks__item-title">Planning Tool</h3>
            In eGo<sup>n</sup>, we will expand the grid planning tool eGo following the established open-source principles. We will connect the electrical grid with additional sectors and integrate more electrical flexibilities.
          </div>
        </div>
      </div>
    </div>
    <div class="small-12 columns">
      <div class="tasks__row row">
        <div class="tasks__item medium-6 columns">
          <div class="tasks__item-text">
          <h3 class="tasks__item-title">Modeling and Complexity</h3>
            There is a conflict between complexity of modeling and accuracy of calculation. Therefore, we will further develop, examine and apply approaches for an adequate reduction of complexity.
          </div>
        </div>
        <div class="tasks__item medium-6 columns">
          <div class="tasks__item-text">
            <h3 class="tasks__item-title">Open Data / Open Source</h3>
            We will follow open-source and open-data principles by exclusively using input data which is freely available and publish own results under open-source and open-data licenses. 
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="openego row row__wrap">
    <div class="columns openego__img">
      <img src="images/open_ego_logo.jpg" alt="Logo open_ego">
    </div>
    <div class="columns openego__text">
      <p>Our previous research project open_eGo with its resulting grid planning tool eGo provides the basis for the current project eGo<sup>n</sup>.  
Incorporating all grid levels, from transmission grid to low-voltage distribution grids, this tool can be used to investigate grid expansion scenarios considering alternative flexibility options such as storages and redispatch. Just like eGo<sup>n</sup>, open_eGo was carried out following the open source and open data principles.
      </p>
      <div class="openego__btn">
        <a href="https://openegoproject.wordpress.com" class="button">See project</a>
      </div>
    </div>
  </section>

  <section class="tools row row__wrap">
    <div class="columns tools__header">
      <h2>Our tools</h2>
    </div>
      {% include _tools.html %}
  </section>

  <section id="anchor-workshops" class="workshops row row__wrap">
    <div class="columns workshops__header">
      <h2>Our workshops</h2>
    </div>
    <div class="small-12 columns">
      <div class="workshops__row row">
        <div class="workshops__item medium-6 columns">
          <div class="workshops__item-text">
            <div class="workshops__item-date">
              September/October 2020
            </div>
            <p>Priorization of research questions, scenarios, assumptions and parameters</p>
            <p>Find the results in <a href="{{ site.url }}{{ site.baseurl }}/publications/#anchor-presentations" title="Publications">Publications</a></p>
          </div>
        </div>
        <div class="workshops__item medium-6 columns">
          <div class="workshops__item-text">
            <div class="workshops__item-date">
              Final workshop: 2<sup>nd</sup> June 2023
            </div>
            <p>In our final workshop we presented our results and introduced our tools and data.</p>
            <p>The workshop was held on 2<sup>nd</sup> June 2023 at the <a href="https://www.schleswig-holstein.de/DE/landesregierung/ministerien-behoerden/LVB/lvb_node.html" title="">Schleswig-Holstein’s Representation in Berlin</a></p>
            <p>Agenda and venue: see <a href="{{ site.url }}{{ site.baseurl }}/presentations/eGon_Abschlussworkshop.pdf" title="program">program</a> (in German). Please note that prior registration is required (free of charge).</p>
            <p>Find the results in <a href="{{ site.url }}{{ site.baseurl }}/publications/#anchor-presentations" title="Publications">Publications</a></p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="funding row row__wrap">
    <div class="columns funding__header">
      <h2>Funding</h2>
    </div>
    <div class="columns funding__text">
      <p>This research project (FKZ: 03EI1002) receives funding within the <a href="https://www.energieforschung.de/energieforschungspolitik/energieforschungsprogramm" title="">7<sup>th</sup> Energy Research Programme</a> by the German Federal Ministry for Economic Affairs and Climate Action from December 2019 until March 2023</p>
    </div>
    <div class="columns funding__logo">
      <a href="https://www.bmwi.de/" title="Zur BMWI Website">
        <img src="images/BMWK.png" alt="Promoted by the Federal Ministry for Economic Affairs and Climate Action">
      </a>
    </div>
  </section>

</div>
