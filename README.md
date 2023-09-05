# DS_Coursera_10_Data_Wrangling
we will review data wrangling. Let’s review some of the attributes: Flight Number, Date, Booster version, Payload mass Orbit, Launch Site, Outcome: this is the status of the first stage Flights, Grid Fins: these help with landing Reused, Legs: used in landing Landing pad, Block, Reused count, Serial, Longitude and latitude of launch Let’s take a look at some of these attributes. The column “LaunchSite” contains the different
launch sites, including: Vandenberg AFB Space Launch Kennedy Space Center CCAFS SLC 40 The column orbits are the different orbits
of the payload. For Example: LEO: Low Earth orbit (LEO)is an Earth-centered
orbit with an altitude of 2,000 km GTO A geosynchronous orbit is a high Earth
orbit that allows satellites to match Earth's rotation. It is located at 22,236 miles (35,786
kilometers) above Earth's equator. The column Outcome indicates if the first
stage successfully landed. There are 8 of them, for example. True ASDS means the booster successfully
landed to a drone ship as shown the following looped video. False ASDS means the mission outcome was
unsuccessfully landed to a drone ship as shown in the video loop. Outcome We would like landing outcomes to be converted
to Classes y.
y. (either 0 or 1). 0 is a bad outcome, that is, the booster did
not land. 1 is a good outcome, that is, the booster
did land. The variable Y will represent the classification
variable that represents the outcome of each launch.
