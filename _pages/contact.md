---
layout: page
permalink: /contact/
title: contact
horizontal: false
nav: true
---
<style>
/* Set the size of the div element that contains the map */
#map {
  height: 400px;
  /* The height is 400 pixels */
  width: 100%;
  /* The width is the width of the web page */
}</style>
<script>
    // Initialize and add the map
function initMap() {
  // The location of Uluru
  const uluru = { lat: -25.344, lng: 131.031 };
  // The map, centered at Uluru
  const map = new google.maps.Map(document.getElementById("map"), {
    zoom: 4,
    center: uluru,
  });
  // The marker, positioned at Uluru
  const marker = new google.maps.Marker({
    position: uluru,
    map: map,
  });
}

window.initMap = initMap;
</script>
<h2>Address</h2>
Mudd Hall <br>
2233 Tech Drive, Third Floor <br>
Evanston, IL 60208
<div id="map"></div>
<script
      src="https://maps.googleapis.com/maps/api/js?key=AIzaSyAPmWWlXbEAkCGlaNN3Ov_cnPVwLgwIAzs&callback=initMap&v=weekly"
      defer
    ></script>
