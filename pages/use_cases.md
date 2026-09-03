---
layout: startpage
title: "Use Cases"
permalink: "/use_cases/"
header: no
---

<div class="page__wrap use-cases">

  <section class="use-cases__header row row__wrap">
    <div class="columns">
      <p class="use-cases__subheading">
        The goal of the reGo<sup>n</sup> project is to bring our tools and datasets into practical application. They are tested in 
        five use cases carried out in close collaboration with practice partners. Together, we define scenario 
        assumptions and validate the results, ensuring that our partners’ requirements are directly reflected in the 
        usability and functionality of the tools.
      </p>
    </div>
  </section>

  <section class="use-cases__items row row__wrap">

    {% include _use_cases.html %}

  </section>

  <section class="use-cases__details row row__wrap">
    {% for uc in site.data._use_cases %}
        <div class="use-cases__detail" id="{{ uc.id }}">
          <div class="use-cases__detail-heading">
            <h3>{{ uc.name }} - {{ uc.title }}</h3>
          </div>
          <div class="use-cases__description-content">
            {{ uc.description }}
            
            {% if uc.research_question %}
              <h4>Research Questions:</h4>
              {% if uc.research_question.first %}
                <ul>
                {% for question in uc.research_question %}
                  <li>{{ question }}</li>
                {% endfor %}
                </ul>
              {% else %}
                <p>{{ uc.research_question }}</p>
              {% endif %}
            {% endif %}
          </div>
          {% if uc.industrial_partners %}
          <div class="use-cases__detail-partners">
            <h4>Practice Partners:</h4>
            <div class="partners-grid">
              {% for industrial_partner_name in uc.industrial_partners %}
                {% assign matched_partner = site.data._industrial_partners | where: "name", industrial_partner_name | first %}
                {% if matched_partner %}
                  <div class="partner__item">
                    <div class="partner__item-upper">
                      <div class="partner__item-name">
                        <a href="{{ matched_partner.url }}" target="_blank"><h3>{{ matched_partner.name }}</h3></a>
                      </div>
                      {% if matched_partner.logo %}
                      <div class="partner__item-img">
                        <a href="{{ matched_partner.url }}" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/{{ matched_partner.logo }}" alt="{{ matched_partner.name }} Logo"></a>
                      </div>
                      {% endif %}
                    </div>
                  </div>
                {% else %}
                  <p><em>No practice partner found for {{ industrial_partner_name }}</em></p>
                {% endif %}
              {% endfor %}
            </div>
          </div>
          {% endif %}
          {% if uc.scientific_partners %}
          <div class="use-cases__detail-partners">
            <h4>Scientific Partners:</h4>
            <div class="partners-grid">
              {% for scientific_partner_name in uc.scientific_partners %}
                {% assign matched_lead = site.data._partners | where: "name", scientific_partner_name | first %}
                {% if matched_lead %}
                  <div class="partner__item">
                    <div class="partner__item-upper">
                      <div class="partner__item-name">
                        <a href="{{ matched_lead.url }}" target="_blank"><h3>{{ matched_lead.name }}</h3></a>
                      </div>
                      {% if matched_lead.logo %}
                      <div class="partner__item-img">
                        <a href="{{ matched_lead.url }}" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/{{ matched_lead.logo }}" alt="{{ matched_lead.name }} Logo"></a>
                      </div>
                      {% endif %}
                      {% if matched_lead.contact %}
                      <div class="partner__item-contact">
                        <p>Contact: <a href="mailto:{{ matched_lead.contact }}">{{ matched_lead.contact }}</a></p>
                      </div>
                      {% endif %}
                    </div>
                  </div>
                {% else %}
                  <p><em>No scientific partner found for {{ scientific_partner_name }}</em></p>
                {% endif %}
              {% endfor %}
            </div>
          </div>
          {% endif %}
        </div>
    {% endfor %}
  </section>

</div>
