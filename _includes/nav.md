<!-- start of nav -->
<div class="header-wrap">
 <div class="container">
  <div id="header-container">
   <div id="header" class="container pt-4">
   <div class="row pt-4">
   <div class="col-6"> <span class="wsite-logo"> <a href="/"> <h1 id="wsite-title">Linda Mezzetti</h1> </a> </span> </div>
   <div class="col-3 text-right mt-4"> <span class="wsite-text wsite-phone"> Contact me and follow me via social media </span> </div>
   <div class="col-1 text-right mt-4"> <span class="wsite-social wsite-social-default"> <a href="https://www.facebook.com/lindapaintsart?ref=hl" target="_blank"><img alt="Linda's facebook link" src="{{ "assets/img/social/facebook-icon-footer.png" | relative_url }} "/></a> <a href="//www.instagram.com/artbymezzetti" target="_blank"><img alt="Linda's instagram link" src="{{ "assets/img/social/instagram-icon-footer.png" | relative_url }} "/></a> </span> </div>
  </div><!-- end row -->
</div><!-- end header -->
</div><!-- end header-container -->
</div><!-- end container -->
</div><!-- end of header-wrap -->
<div class="main-wrap">
<div class="container">
<style>
/* Dropdown Content (Hidden by Default) */
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #002e53;
  color:white;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
  width:100%;
  line-height:2rem;
  top:32px
}

/* Links inside the dropdown */
.dropdown-content a {
  color: white;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

/* Change color of dropdown links on hover */
.dropdown-content a:hover {background-color: #fff;
    color: #001e36;
}

/* Show the dropdown menu on hover */
.dropdown:hover .dropdown-content {display: block;}

/* Change the background color of the dropdown button when the dropdown content is shown */
.dropdown:hover .dropbtn {background-color: #001e36;}
</style>
<script>
$(document).ready(function(){
    $("#toggleLink").unbind().click(function() {
        var showList = $("#toggleLink").hasClass("show-nav-link");
        if (showList) {
            $("#sub-menu").show();
            $("#toggleLink").removeClass("show-nav-link");
            $("#toggleLink").addClass("hide-nav-link");
            $("#toggleLink").html("Hide section navigation<span class=\"fa fa-angle-up\">&nbsp;</span>");
        } else {
            $("#sub-menu").hide();
            $("#toggleLink").removeClass("hide-nav-link");
            $("#toggleLink").addClass("show-nav-link");
            $("#toggleLink").html("Show section navigation<span class=\"fa fa-angle-down\">&nbsp;</span>");
        }
    });
});
</script>
<nav id="topnav" role="navigation"><!-- class="collapse navbar-collapse">-->
   <ul class="wsite-menu-default"><!-- nav navbar-nav">-->
   <li id="menu-about" class=""> <a href="{{ "/" | relative_url }}">ABOUT ME</a> </li>
   <li id="menu_dropdown-menu" id="" class="dropdown"> <a href="{{ "gallery" | relative_url }}" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">GALLERY <span class="caret"></span></a>
<ul class="dropdown-content">
<li> <a href="{{ "gallery/acrylic-paintings.html" | relative_url}}">Acrylic Paintings</a> </li>
<li> <a href="{{ "gallery/oil-paintings.html" | relative_url}}">Oil Paintings</a> </li>
<li> <a href="{{ "gallery/silk-paintings.html" | relative_url}}">Silk Paintings</a> </li>
<li> <a href="{{ "gallery/thumbnails.html" | relative_url}}">Acrylic Thumbnails</a> </li>
</ul><!-- end dropdown-->
   </li><!-- end dropdown-menu-->
            
<li id="se" class=""> <a href="{{"showsexhibitions" | relative_url}}">SHOWS AND EXHIBITIONS</a> </li>

<li id="sc" class=""> <a href="{{"sewing" | relative_url}}">SEWN CREATIONS</a> </li>

<li id="cm" class=""> <a href="{{"contact" | relative_url}}">CONTACT ME</a> </li>
</ul>
</nav>
<!-- end of nav -->

