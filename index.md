---
layout: article
aside:
  toc: false
#mode: immersive
#article_header:
#  type: overlay
#  theme: dark
#   background_color: "#203028"
#   background_image:
#     gradient: "linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))"
#     #src: /docs/assets/images/cover3.jpg
#     src: /assets/logo.png
---

<div class="index_container">
  <img class="index_image" src="{{ site.baseurl }}/assets/images/Sala%20A.jpeg">
  <div class="index_text">
    <h3>Dolmen studio</h3>
    dal 1996 con una passione unica per la Musica.
    <p>
      In oltre dieci anni di attività, questa passione, insieme alla cura del dettaglio, all’attenzione nella scelta della strumentazione e alla disponibilità nell'assistenza agli artisti, ci ha permesso di creare un vero e proprio laboratorio aperto a tutti i musicisti, dagli appassionati alle prime armi ai professionisti più esigenti.
    </p>
  </div>
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
