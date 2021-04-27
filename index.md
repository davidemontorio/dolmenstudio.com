---
layout: article
aside:
  toc: false
---

<div class="index_container">
  <img class="index_image" src="{{ site.baseurl }}/assets/images/Sala_A.jpeg">
  <div class="index_text">
    <h3>Dolmen studio</h3>
    dal 1996 con una passione unica per la Musica.
    <p>
      In oltre dieci anni di attività, questa passione, insieme alla cura del dettaglio, all’attenzione nella scelta della strumentazione e alla disponibilità nell'assistenza agli artisti, ci ha permesso di creare un vero e proprio laboratorio aperto a tutti i musicisti, dagli appassionati alle prime armi ai professionisti più esigenti.
    </p>
  </div>
</div>
<div>
    <ul class="index_menu">
{%- for _item in site.data.navigation.header -%}
  {%- include snippets/get-nav-url.html path=_item.url -%}
  {%- assign _nav_url = __return -%}
  {%- include snippets/get-nav-url.html path=page.url -%}
  {%- assign _page_url = __return -%}
  {%- include snippets/get-string-from-locale-config.html locale=_item.titles -%}
  {%- if _nav_url == _page_url or page.nav_key and _item.key and page.nav_key == _item.key -%}
    <li class=" navigation__item--active"><a href="{{ _nav_url }}">{%- if _item.title -%}{{ _item.title }}{%- else -%}{{ __return }}{%- endif -%}</a></li>
  {%- else -%}
    <li class=""><a href="{{ _nav_url }}">{%- if _item.title -%}{{ _item.title }}{%- else -%}{{ __return }}{%- endif -%}</a></li>
  {%- endif -%}
{%- endfor -%}
    </ul>
</div>

<style>
  .index_container {
      width: 100%;
      display: flex;
    }
    .index_image {
      margin: 20px 30px 0 0;
      width: 50%;
      float: left;
      object-fit: contain;
      align-self: flex-start;
    }
    .index_text {
      flex: 1 1 auto;
      vertical-align: middle;
    }
  @media only screen and (max-width: 767px) {
    .index_container {
      width: 100%;
      display: block;
    }
     .index_image {
      margin: 20px 30px 0 0;
      width: 100%;
      float: none;
     }
    
  }
  .col-aside{
    display: none !important;
    visibility: hidden !important;
  }
</style>
