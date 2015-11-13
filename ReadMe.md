# Project title
## Data Representation and Querying Project 2015
### Neil Kyne

## Introduction
This project provides the design and documentation for the dataset "Roscommon Fire Stations" which is available at [https://data.gov.ie/]

The type of people I think will use the app are people who are unsure about how many fire stations are in Roscommon or how close they are to one if there was ever situation where they would need one. The app will provide all this information and more.

## About the data
This dataset was received in Comma Separated Values (CSV) format, and was downloaded from [https://data.gov.ie/dataset/roscommon-fire-stations8b29d/resource/1c8e2cae-af21-4eda-b6ea-2c187a2099dc]

This dataset gives us information about every fire station in county Roscommon. From their address to their coordinates on a map, to their phone and emails.

The CSV file contains 7 rows and 19 columns, the first being a header row with the names of each field.
There are 16 values on each line, which are as follows:
    A - ** X **: The position the fire station is on the x axis of a map of Ireland.
    B - ** Y **: The position the fire station is on the y axis of a map of Ireland.
    C - ** ObjectID **: The ID of each object in the data set.
    D - ** ID **: Again, the ID of each object in the data set.
    E - ** Coucil_ID **: The ID of the coucil the fire station is under. In this case 'RN' for Roscommon.
    F - ** Administrative_Authority **: The administration that has authority over the fire stations. Again it's Roscommon County Council.
    G - ** Name **: The name of the fire station.
    H, I - ** Address_1 / Address_2 **: The address of the station.
    J - ** Town **: The town the fire station is situated in.
    K - ** County **: The town the fire station is situated in.
    L, M - ** Phone / Email **: The phone number and email for the station.
    N, O - ** Website, Image **: The website and link to images of the fire station.
    P - ** WGS84 Latitude **: Coordinates on a map for latitude.
    Q - ** WGS84 Longitude **: Coordinates on a map for longtitude.
    R - ** Streetview_Link **: A link for google streetview to see the stations up close.
    S - ** Eircode **: The Eircode of each station.
    
## Design of the app
In my opinion the app will appeal to older generations rather than younger ones. I just believe young people are more carefree and less concerned about this type of thing then older generations, therefore, I believe the app should be extremely user friendly and really easy to use. Not to assume that older people are any worse with technology but I think younger people can probably navigate more complicated apps easier.

## Menu
I think the menu that the user will see the second they open the app will look like this. We will be brought straight into the list of stations, and then if the user wished to search for a specific station, they can click the star (settings) button at the top right of the screen.
    
Here is an example of how the app will look straight off:

https://static.dyp.im/S3DM9qXDLO/15006fc682be267fead6299660184596.png
    
## Search(Star)
The search button (the star) will be very simple too. Once clicked a search bar will appear on a side menu. There, a user can search by either town, name, address or eircode.
    
    
Here is an example of how the search bar will look:
    
https://static.dyp.im/Qz1EBpHdha/2b021a1b71d8a03368eecbbc64ba8048.png

## Map
Although I'm not big on maps in apps this one probably could hae one. We're given longtitue and latitude coordinates so it wouldn't be difficult to incorporate one.
    
## URl's
One of the URL's could be a list of stations that are a certain size. For example, if we were to have a url like the following:

List of large fire stations (stations with 2 or more trucks and over 10 members):

*http://roscfirestations.com/size/[large]*
where you replace [large] with the size of the station.
For example, the URL:
*http://roscfirestations.com/large
will return a list of large stations in Roscommon.

The size of the stations could be decided by how many fire trucks they have and how many active members they have.

List of small fire stations (stations with 1 truck and less than 10 members):

*http://roscfirestations.com/size/[small]*
where you replace [small] with the size of the station.
For example, the URL:
*http://roscfirestations.com/small
will return a list of small stations in Roscommon.

List of fire stations in a specific area:

*http://roscfirestations.com/area/[area]*
where you replace [area*] with an address or town.
For example, the URL:
*http://roscfirestations.com/area/Boyle
will return a list of stations in the town of Boyle

We could now easily mix these two together. If we wanted to find only small stations in a certain are we can combine the two, like so:
List of small fire stations in a specific area:

*http://roscfirestations.com/area-size/[area-size]*
where you replace [area-size*] with an address or town and which size you want.
For example, the URL:
*http://roscfirestations.com/area-size/Boyle-small
will return a list of small stations in the town of Boyle

List of large fire stations in a specific area:

*http://roscfirestations.com/area-size/[area-size]*
where you replace [area-size*] with an address or town and which size you want.
For example, the URL:
*http://roscfirestations.com/area-size/Boyle-large
will return a list of large stations in the town of Boyle








    
    
    
    
    
    