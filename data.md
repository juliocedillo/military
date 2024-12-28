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

  // Add a marker for Fort Knox, KY
  L.marker([37.9161, -85.9562]).addTo(map)
    .bindPopup("<b>Fort Knox, KY</b><br>Hispanic/Latino: 25.1%")
    .openPopup();
</script>

