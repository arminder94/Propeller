<!DOCTYPE html>
<html>
<head>
<title>Propeller</title>
<link href="css/style.css" rel="stylesheet" type="text/css"/>  
</head>
<body>

<div class="wrapper">
<button class="accordion">Section 1</button>
<div class="panel">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore sed aliquam vitae 
  fugit odit voluptate eligendi, blanditiis quasi nobis reiciendis! Rem maiores 
  reprehenderit animi aliquam inventore vel adipisci delectus itaque! Lorem ipsum dolor 
  sit amet, consectetur adipisicing elit. Tempore sed aliquam vitae fugit odit voluptate
   eligendi, blanditiis quasi nobis reiciendis!</p>
</div>

<button class="accordion">Section 2</button>
<div class="panel">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore sed aliquam vitae
   fugit odit voluptate eligendi, blanditiis quasi nobis reiciendis! Rem maiores
    reprehenderit animi aliquam inventore vel adipisci delectus itaque! Lorem ipsum dolor
     sit amet, consectetur adipisicing elit. Tempore sed aliquam vitae fugit odit
      voluptate eligendi, blanditiis quasi nobis reiciendis! Rem maiores reprehenderit
       animi aliquam inventore vel adipisci delectus itaque!</p>
</div>

<button class="accordion">Section 3</button>
<div class="panel">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>
</div> 


<script>
var acc = document.getElementsByClassName("accordion");
var i;

for (i = 0; i < acc.length; i++) {
    acc[i].addEventListener("click", function() {
        this.classList.toggle("active");
        var panel = this.nextElementSibling;
        if (panel.style.display === "block") {
            panel.style.display = "none";
        } else {
            panel.style.display = "block";
        }
    });
}
</script>

</body>
</html>
