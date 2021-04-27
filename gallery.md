---
layout: article
aside:
  toc: false
---

# Gallery

{% include image-gallery.html folder="/assets/images" %}

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
