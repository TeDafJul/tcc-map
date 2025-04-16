// ---- MAP INITIALIZATION ----

// 1. Create the map object, targeting the 'map' div, set initial view and zoom
// Coordinates are [latitude, longitude]
// Zoom level: 1 is zoomed out (world), ~13 is city level, ~18 is block level
const map = L.map('map').setView([20, 0], 2); // Centered roughly, zoomed out

// 2. Add the Tile Layer (the map images)
// Using OpenStreetMap's free tile server
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '© <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
}).addTo(map);

// ---- LOCATION DATA ----
// This is where you add information for each pin!
// Structure: { lat: NUMBER, lng: NUMBER, name: "STRING", description: "STRING" }

const locations = [
    {
        lat: 35.6895,       // Latitude of Tokyo
        lng: 139.6917,      // Longitude of Tokyo
        name: "Alice",      // Name of the person (or place identifier)
        description: "Grew up in Tokyo! 🇯🇵" // A short description shown in the popup
    },
    {
        lat: 48.8566,       // Latitude of Paris
        lng: 2.3522,        // Longitude of Paris
        name: "Bob",
        description: "Lived in Paris for 5 years. 🥐🇫🇷"
    },
    {
        lat: -33.8688,      // Latitude of Sydney
        lng: 151.2093,      // Longitude of Sydney
        name: "Charlie",
        description: "Born in Sydney. ☀️🇦🇺"
    },
    {
        lat: 19.4326,       // Latitude of Mexico City
        lng: -99.1332,      // Longitude of Mexico City
        name: "Diana",
        description: "Family is from Mexico City. 🌮🇲🇽"
    }
    // --- ADD MORE LOCATIONS HERE ---
    // Copy the block below and paste it above this comment, then edit the details.
    /*
    ,{ // Don't forget the comma if adding before others!
        lat: 0.0000,        // <-- Replace with Latitude
        lng: 0.0000,        // <-- Replace with Longitude
        name: "New Person", // <-- Replace with Name
        description: "Tell us about this place!" // <-- Replace with Description
    }
    */
];


// ---- ADDING MARKERS TO THE MAP ----

// Loop through each location in the 'locations' array
locations.forEach(location => {
    // Create a marker for the current location
    const marker = L.marker([location.lat, location.lng]).addTo(map);

    // Create the popup content (HTML works here!)
    const popupContent = `<b>${location.name}</b><br>${location.description}`;

    // Bind the popup to the marker (so it shows when clicked)
    marker.bindPopup(popupContent);
});

console.log("Map initialized and markers added!"); // A message for the browser's developer console