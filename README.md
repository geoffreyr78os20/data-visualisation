# data-visualisation

This repo contains two simple html files, both files must be run on a server in order for the data to be displayed.

index.html uses the D3 library to present the total number of covid 19 cases in a bar chart drawn in an svg.
I have created an input box that can be used to filter the data displayed by date, e.g. 2020-13-05.

index02.html then explores the idea of combining the D3 library with the Aframe VR framework, 
this works in the exact same way as the first file.

I encountered one bug that I was unable to solve which exists in both files, this took place when trying to filter data for a second time.
When creating a new bar chart with new data, the orignal bar chart would not delete and instead 
a new bar chart would be placed on top of the previous.

I tried to solve this issue by re organising my code in and placing it into an update function however that did not seem to work.
After looking further into this matter I believe the problem lies within line 86 of the index.html file.
Another possible soloution to fix this, was to create a second button that would reset the filtered data or combining the d3 library with react
and have it work with react states.
