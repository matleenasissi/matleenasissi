
<!DOCTYPE html>
<html lang="fi">
<head>
  <title>Matleenan makramee</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">
  <!-- linkki google-fonttiin -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Catamaran:wght@100&display=swap" rel="stylesheet">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
     <style>
body {font-family: 'Catamaran', sans-serif;
      background-color: rgba(244,244,244, 0.8);
      position: relative;
         text-align: center;}

 /* taustan väri */
.navbar-custom {
    background-color: rgba(192,75,24, 0.8);
    border-radius: 50px
    
}

/* brandin ja tekstin väri */
.navbar-custom .navbar-brand,
.navbar-custom .navbar-text{
    color: rgba(0,0,0,0.8);
    
}

/* linkin väri */
.navbar-custom .navbar-nav .nav-link {
    color: black;
}

/* aktiivisen & hover-linkin väri */
.navbar-custom .nav-item.active .nav-link,
.navbar-custom .nav-item:hover .nav-link {
    color: #ffffff;
}


/* hampurilaiskuvion (svg-kuva) värin */
.custom-toggler .navbar-toggler-icon {
  background-image: url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 32 32' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath stroke='rgba(0,0,23, 0.5)' stroke-width='2' stroke-linecap='round' stroke-miterlimit='10' d='M4 8h24M4 16h24M4 24h24'/%3E%3C/svg%3E");
}

/* alasvetovalikko hover-tausta */
 .nav-item .dropdown-menu a:hover {
            color: white !important;
            background: grey !important;
            cursor: pointer;
  }
      
/* scroll spy */
.nav-link.active {
	  color: white !important;
	}        
      
/* karuselli */
.carousel-inner img {
     
      height:100%;
      margin: auto;
      display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
     
      }
      
         .alaskuva {
     
      height:100%;
      margin: auto;
      display: block;
  margin-left: auto;
  margin-right: auto;
  width: 70%;
border-radius: 25px 0 25px 0;
     
      }
      
.jumbotron {background-color: rgba(249,188,75,1);
            color:  black;}
      
/* hieman tilaa osion yläosaa ettei se navigoidessä jää navipalkin taakse */
#info, #demo, #accordion, #yhteydenotto {padding-top:50px;}
      

/* navipalkki ja sisältö samaan linjaan */
.container {
padding: 10px 0px;
}
.navbar img {margin-left:10px !important;}

 a.nav-link {margin-left:5px !important;}

/* haitarin kuvat */
      .juomat img {width:100%; 
                  max-width: 450px;}
  
      fieldset {border: 1px dotted rgba(249,110,110,0.9);
               padding: 10px;
               width:100%;
               max-width: 45em;
               margin-bottom:20px;
               margin:auto;}
    input {color:rgba(13,17,76,0.9);
             border:rgba(249,188,175,1) 1px solid;}
      input[type=submit],input[type=reset]{color:bisque; 
            background-color:rgba(249,110,110,1);}
         
         /* Popup ennen klikkausta */
.popup {
  position: relative;
  display: inline-block;
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  color: rgba(192,75,24, 0.8);
    font-family: 'Catamaran', sans-serif;
    
   
 
}

/* Itse popup */
.popup .popuptext {
  visibility: hidden;
  width: 160px;
  background-color: #565;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 8px 0;
  position: absolute;
  z-index: 1;
  bottom: 125%;
  left: 50%;
  margin-left: -80px;
}

/* Popup arrow */
.popup .popuptext::after {
  content: "";
  position: absolute;
  top: 100%;
  left: 50%;
  margin-left: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: #555 transparent transparent transparent;
}

/*popup */
.popup .show {
  visibility: visible;
  -webkit-animation: fadeIn 1s;
  animation: fadeIn 1s;
}

/* Animaatio */
@-webkit-keyframes fadeIn {
  from {opacity: 0;} 
  to {opacity: 1;}
}

@keyframes fadeIn {
  from {opacity: 0;}
  to {opacity:1 ;}
}
         .accordion {

  cursor: pointer;
  padding: 18px;
  width: 50%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
  transition: 0.4s;
}

.aktiivinen, .accordion:hover {
background-color: rgba(192,75,24, 0.8);
}

.panel {
  padding: 0 18px;
  display: none;
    width: 50%;
margin: auto;
}
         
         footer {
  text-align: center;
  padding: 3px;
    

}
        #myDIV {
  width: 100%;
  height: 90px;
  background: lightcoral;
  animation: mymove 5s infinite;
        
}

@keyframes mymove {
   0%   {background-color: sandybrown;}
  25%  {background-color: rgba(255,165,0,0.8);}
  50%  {background-color: rgba(239,178,97,0.8);}
  100% {background-color: rgba(252,172,3,0.8);}
}
  </style>
  
</head>
<body data-spy="scroll" data-target=".navbar" data-offset="50" onload="loadMap()">

<div class="container" id="alku">
  <nav class="navbar navbar-expand-lg navbar-custom fixed-top container">
	<a class="navbar-brand" href="#alku"><img src="logoa.png" alt="logo" style="width:40px;"> Matleenan makrameet</a>

<button class="navbar-toggler custom-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    	<span class="navbar-toggler-icon"></span>
  	</button>

  	<div class="collapse navbar-collapse" id="navbarSupportedContent">
    	<ul class="navbar-nav mr-auto">
      	<li class="nav-item">
<a class="nav-link" href="#demo">Etusivu</a>
      	</li>
      	<li class="nav-item">
        <a class="nav-link" href="#tilaus">Tilaus</a>
      	</li>
      
            
      <li class="nav-item">
        <a class="nav-link" href="#yhteydenotto">Ota yhteyttä</a>
      </li>
    </ul>
    
     </div>
     </nav>
    
    <!-- KARUSELLI -->
    
    <div id="demo" class="carousel slide" data-ride="carousel">
  <ul class="carousel-indicators">
    <li data-target="#demo" data-slide-to="0" class="active"></li>
    <li data-target="#demo" data-slide-to="1"></li>
   
  </ul>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="kuva10.jpg" alt="seinavaate" width="250" height="450">

      <div class="carousel-caption">
        <h3>Makramee seinävaatteet</h3>
        <p>Näyttävät seinävaatteet monissa väreissä.</p>

      </div>   
    </div>


      
    <div class="carousel-item">
      <img src="kuva4.jpg" alt="amppelit">
      <div class="carousel-caption">
        <h3>Värikkäät makramee amppelit</h3>
        <p>Saatavilla myös syksyisissä sävyissä.</p>
      </div>   
    </div>
      <br>
  </div>
  <a class="carousel-control-prev" href="#demo" data-slide="prev">
    <span class="carousel-control-prev-icon"></span>
  </a>
  <a class="carousel-control-next" href="#demo" data-slide="next">
    <span class="carousel-control-next-icon"></span>
  </a>
</div>
    
    <!-- info: jumbotron -->
<div class="container-fluid" id="tilaus">
  <div class="jumbotron">
 
  
    <div class="container">
     <div class="row">
         
   
    <!--  lomake -->
        
    <div class="col-sm-6">
    <form onsubmit="return false">
    <fieldset>
       <h3>Tilaa</h3>
        <label>Nimi:
    
        <input type="text" required id="nimi2">
        </label> <br>
        <label>Sähköposti:
        <input type="email" required id="email2">
        </label><br>
       Haluatko tilata? <br>
        <label>
         <input type="radio" name="kumpi" value="Seinävaatteen">Seinävaatteen
        </label>
         <label>
         <input type="radio" name="kumpi" value="Amppelin"> Amppelin
        </label> <br>
         
        Lankojen värit:<br>
        <label>
         <input type="checkbox" name="lisaa" value="Valkoinen"> Valkoinen
        </label>
          <label>
         <input type="checkbox" name="lisaa" value="Vaaleanpunainen"> Vaaleanpunainen
        </label><br>
            <label>
         <input type="checkbox" name="lisaa" value="Sinapinkeltainen"> Sinapinkeltainen
        </label> 
           <label>
         <input type="checkbox" name="lisaa" value="Beige"> Beige
        </label> <br>
        Tuotteen koko:<br>
        <select id="koko">     
          <option value="Pieni">Pieni</option>
          <option value="Suuri">Suuri</option>
        </select>
        <br><br>
        <input type="submit" value="lähetä" onclick="palaute()">
        <input type="reset" value="tyhjennä">
        </fieldset>
        <br>


    </form>
        
    </div>
        
          <div class="col-sm-6">
    <form onsubmit="return false" >
    <fieldset>
     
     <h3>Anna palautetta: </h3>
        <label for="nimi" class="muoto">Nimi:</label> 
     <input type="text" required id="nimi">
    <br>
        <label for="email" class="muoto">Sähköposti:</label>
     <input type="email" id="email" required>
   
     <label class="muoto" for="toive"></label> <br>
         <textarea placeholder=" Kirjoita palaute..." id="toive"></textarea>
      <br>
      <label class="muoto"> </label>
     <input type="submit" value="lähetä" onclick="varaus()">
     <input type="reset" value="tyhjennä">
   
    </fieldset> <br>
        <button>Katso värivaihtoehdot</button><br><br>

<div id="div1" style="width:80px;height:80px;display:none;background-color:ivory;float:left;"></div>
<div id="div2" style="width:80px;height:80px;display:none;background-color:lightcoral;float:left;"></div>
<div id="div3" style="width:80px;height:80px;display:none;background-color:rgba(253,188,0);float:left;"></div>
    <div id="div4" style="width:80px;height:80px;display:none;background-color: rgb(245, 245, 220);float:left;">
    </div>
    </form>
        
        
    <!-- tulostetaan lomakkeen tiedot -->
    <div id="varaustiedot"></div>
    </div>
    
    </div>
    </div></div>

   
      <img src="makramee.jpg"  class="alaskuva" alt="makrameesiivet">
    </div>
    

  </div>
    
<div class="popup" onclick="myFunction()">Klikkaa nähdäksesi vinkki makrameen tekoon.
  <span class="popuptext" id="myPopup">Vältä tyypilliset virheet: <br>
-Älä jätä solmuja löysäksi
<br>
-Tehdessäsi isoa seinävaatetta solmi langat nippuun 
</span>
</div>


<h2>Lisätietoa käytetyistä materiaaleista</h2>

<button class="accordion">Langat</button>
<div class="panel">
  <p>Langat ovat aina suomessa valmistettuja ja niiden värjäämiseen on käytetty aina luonnon omia väriaineita.</p>
</div>

<button class="accordion">Puiset osat</button>
<div class="panel">
  <p>Puiset osat ovat tammea. Tammea on kohdeltu varoen ja mukaillen sen omaa luonnollista muotoa. Tämän vuoksi jokainen seinävaate on yksilöllinen.</p>
</div>

<button class="accordion">Ruukut</button>
<div class="panel">
  <p>Tulevaisuudessa on tarkoitus, että tilaajalla on mahdollisuus saada saviruukku amppelin mukana. Saviruukut ovat käsintehtyjä.</p>
</div>

<script>
var acc = document.getElementsByClassName("accordion");
var i;

for (i = 0; i < acc.length; i++) {
  acc[i].addEventListener("click", function() {
    this.classList.toggle("aktiivinen");
    var panel = this.nextElementSibling;
    if (panel.style.display === "block") {
      panel.style.display = "none";
    } else {
      panel.style.display = "block";
    }
  });
}
</script>

    
    <!-- taulukko -->
    
    <div class="table-responsive" id="yhteydenotto">
    <table class="table">
      <thead>
        <tr>
          <th>Nimi</th>
          <th>Tehtävä</th>
          <th>Puhelin</th>
          <th>Sähköposti</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Matleena&nbsp;Sissi</td>
          <td>Toimitusjohtaja</td>
          <td>0440440440</td>
          <td>matleena.sissi@haaga-helia.fi</td>
        </tr>
          <tr>
          <td>Hessu&nbsp;Hopo</td>
          <td>Tuotesuunnittelija</td>
          <td>0440440400</td>
          <td>hessu.hopo@haaga-helia.fi</td>
        </tr>         
         <tr>
          <td>Hauska&nbsp;Heppu</td>
          <td>Asiakasvastaava</td>
          <td>0440440444</td>
          <td>hauska.heppu@haaga-helia.fi</td>
        </tr>
      </tbody>
    </table>
  </div>
    
    <h2>Kivijalkamyymälän osoite</h2>
    <div id = "map" style = "width:400px; height:400px;display: block;
                             margin-left: auto;margin-right: auto;width: 50%;"></div>
      <script>

        // fake JSON call
        function getJSONMarkers() {
          const markers = [
            {
              
              name: "Kauppa",
              location: [60.5398491,24.2247522]
            }
          ];
          return markers;
        }

        function loadMap() {
          // Initialize Google Maps
          const mapOptions = {
            center:new google.maps.LatLng(60.5398491,24.2247522),
            zoom: 11
          }
          const map = new google.maps.Map(document.getElementById("map"), mapOptions);

          // Load JSON Data
          const hotelMarkers = getJSONMarkers();

          // Initialize Google Markers
          for(hotel of hotelMarkers) {
            let marker = new google.maps.Marker({
              map: map,
              position: new google.maps.LatLng(hotel.location[0], hotel.location[1]),
              title: hotel.name
            })
          }
        }
      </script>
      <script src = "https://maps.googleapis.com/maps/api/js"></script>
  

<script>
// When the user clicks on div, open the popup
function myFunction() {
  var popup = document.getElementById("myPopup");
  popup.classList.toggle("show");
}
</script>
    <script>$(document).ready(function(){
  $("button").click(function(){
    $("#div1").fadeIn();
    $("#div2").fadeIn("slow");
    $("#div3").fadeIn(200);
      $("#div4").fadeIn(3000);
  });
});
    </script>

      
      
   <script>
    function varaus(){
        var nimi = document.getElementById("nimi").value;
        var sposti = document.getElementById("email").value;
        // tähän vielä muiden lomake-elementtien tietojen lukeminen samalla lailla
        // tulostetaan tiedot div-elementtii
        document.getElementById("varaustiedot").innerHTML="Kiitos palautteesta "+nimi+"<br>Sähköpostisoitteesi: "+sposti;
    }
       
     function palaute(){
         var taulukko=[];
         taulukko.push("Kiitos tilauksesta. ");
         // radiobuttonit     
        var radios = document.getElementsByName("kumpi");
         // checkboxit
         var boxit = document.getElementsByName("lisaa");
         // radiot
        for (var i=0, length = radios.length; i<length; i++){
            if (radios[i].checked){
                taulukko.push(" Tilasit:  "+radios[i].value+", ");
                break;
            }
        }
         // checkboxit
      taulukko.push(" Väri: "); 
      for (var i=0, length = boxit.length; i<length; i++){
            
            if (boxit[i].checked){
                taulukko.push(boxit[i].value + ", ");
                
            }
        }
        
         
         // alasvetovalikko
         var x = document.getElementById("koko").selectedIndex;
         var y = document.getElementById("koko").options;
         taulukko.push("Tuotteen koko: " + y[x].text); 
         
          // yhdistetään taulukon solut tulostusta varten
         alert(taulukko.join(" "));
     }
    </script>
    <!-- The core Firebase JS SDK is always required and must be listed first -->

    <br>
    <div id="myDIV">
<footer>
    
     <p>Kysy rohkeasti lisätietoja:<br>
  <a href="matleena.sissi@haaga-helia.fi">matleena.sissi@haaga-helia.fi</a></p>
</footer></div>
    </body>
</html> 
