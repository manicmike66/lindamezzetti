---
title: "Art Thumbnails"
layout: "normal"
keywords: "Linda Mezzetti, Melbourne, Australia, painting"
description: "Display of all her paintings"
---
<div class="container-md">
<div class="row">
{% for painting in site.data.paintings %}
<div class="col-md-1" data-toggle="modal" data-target="#myModal"><a href="#myGallery" data-slide-to="{{painting.file}}"><img style="height:70%;width:auto" src="../assets/img/{{ painting.type }}/{{ painting.file}}.jpg" class="img-thumbnail" /></a></div>
{% endfor %}
<!--<li data-toggle="modal" data-target="#myModal">
<a href="#myGallery" data-slide-to="0"><img style="height:10%;width:10%" src="{{ "../assets/img/acrylics/0.jpg" | relative_url}}" class="img-thumbnail" /></a>
</li>
<li data-toggle="modal" data-target="#myModal"><a href="#myGallery" data-slide-to="1"><img style="height:10%;width:10%" src="{{ "../assets/img/acrylics/1.jpg"|relative_url }}" class="img-thumbnail" /></a></li>-->
<!-- The Modal -->

<div class="modal" id="myModal">

<div class="modal-dialog">

<div class="modal-content"> 

<!-- Modal Header -->

<div class="modal-header"> <h4 class="modal-title">Full-size version</h4> <button type="button" class="close" data-dismiss="modal">&times;</button> </div>

<!-- Modal body -->

<div class="modal-body"> 

<!--INSERT CAROUSEL & FULL SIZE IMAGES HERE-->

<div id="myGallery" class="carousel slide bg-dark" data-ride="carousel"  data-interval="false" > 
<div class="carousel-inner" role="listbox"> 
<div class="container">
<div class="row">
{% for painting in site.data.paintings %}
<div {% if painting.file == 0%} class="col carousel-item active" {% else %} class="col carousel-item" {% endif %}> <img class="mx-auto" src="../assets/img/{{ painting.type }}/{{ painting.file }}.jpg" alt="{{ painting.title }}"> 
<div class="carousel-caption" style="right:60%;left:0;"> <h5>{{ painting.title }}</h5> <p>{{ painting.desc }} {{ painting.size}}</p> </div><!--end-caption-->
</div><!--end-item-->
{% endfor %}
</div><!-- end row -->
</div><!-- end container -->
</div><!--end-inner-->

<!--Previous & Next arrows-->

<a class="carousel-control-prev" href="#myGallery" role="button" data-slide="prev"> <span class="carousel-control-prev-icon" aria-hidden="true"></span> <span class="sr-only">Previous</span> </a> <a class="carousel-control-next" href="#myGallery" role="button" data-slide="next"> <span class="carousel-control-next-icon" aria-hidden="true"></span> <span class="sr-only">Next</span> </a> </div><!--end-inner-->

</div><!--end-carousel-->

<div class="modal-footer">


<button type="button" class="btn btn-danger" data-dismiss="modal">Close</button>

</div><!-- end modal-footer -->


</div><!--end-modal-body-->
<!-- end width -->

