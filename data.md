---
layout: default
title: Data
permalink: /data
---

<head>
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" />
  <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script>
</head>

# Areas of Interest

<div id="mapid" style="height: 500px;"></div> <!-- Increased height for better visibility -->

<script>
  // Initialize the map and center it on the US
  var map = L.map('mapid').setView([39.8283, -98.5795], 5); // Centered on the US with zoom level 5

  // Add OpenStreetMap tiles
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
  }).addTo(map);

  L.marker([37.9161, -85.9562]).addTo(map)
    .bindPopup("<b>Fort Knox</b><br>Fort Knox, KY")
    .openPopup();

  L.marker([33.2145, -117.3872]).addTo(map)
    .bindPopup("<b>Camp Pendleton</b><br>San Diego, CA")
    .openPopup();

  L.marker([31.1551, -97.7646]).addTo(map)
    .bindPopup("<b>Fort Cavazos (Fort Hood)</b><br>Killeen-Copperas Cove, TX")
    .openPopup();

  L.marker([35.139167, -78.999167]).addTo(map)
    .bindPopup("<b>Fort Liberty (Fort Bragg)</b><br>Fayetteville, NC")
    .openPopup();

 L.marker([32.8115, -115.6723]).addTo(map)
    .bindPopup("<b>Naval Air Facility El Centro</b><br>El Centro, CA")
    .openPopup();  

L.marker([32.887299, -117.119843]).addTo(map)
    .bindPopup("<b>Marine Corps Air Station Miramar</b><br>San Diego, CA")
    .openPopup();  
</script>

