# Wake County Greenway Plan Map

Wake County, NC has an official greenway plan, which can be found [here](https://altago.com/wp-content/uploads/Wake-County-Greenway-System-Plan.pdf). However, it is not interactive, and doesn't show high detail.

Each town also has their own plans for greenways and other pedestrian areas, but they are each in their own separate map, and most are not interactive.

I wanted a way to see all this information in one place, interactively. So I created this map.

## How it was made

1. Download each of the individual town maps:
  - [Cary](https://www.carync.gov/home/showpublisheddocument/14421/636507369979070000)
  - [Holly Springs](https://www.hollyspringsnc.gov/DocumentCenter/View/33575/Master-Plan-Proposed-Greenway-Trails-AND-Community-connectors)
  - [Fuquay-Varina](https://online.flippingbook.com/view/880718258/132-133/#zoom=true)
  - [Apex](https://www.apexnc.org/DocumentCenter/View/3722/Parks-Recreation-Greenways-and-Open-Space-Master-Plan-Map-?bidId=)
2. Convert the PDF to PNG, using [this site](https://pdf2png.com/)
3. Crop the image to only include the map
4. Show the map via [Leaflet's ImageOverlay](https://leafletjs.com/reference.html#imageoverlay)
5. Position the map, by obtaining rough coordinates based on visual inspection, then adjusting.
6. Edit the photos using [Photopea](https://www.photopea.com/) (a free photoshop clone). Use magic wand to select specific colors for the greenway trails and whatnot. Invert selection, delete. Export PNG
7. Swap the displayed image for the new one with only the important parts.
