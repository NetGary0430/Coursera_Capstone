# Relocating with Foursquare

**Introduction**:

I have the opportunity to relocate. My choice, however, will revolve
around the selection of restaurants and the performing arts available in
the new locations.

I have lived in places such as Chicago that have a plethora of food
options. I have also lived places where my options were limited to
Subway, McDonald's, and a couple of teriyaki joints. As I want this to
be my last move - I am nearing retirement - I want to find a
comfortable, compatible city to match my wants and needs.

Additionally, I really enjoy walking through museums and attending live
performances. I am currently reviewing job offers from two firms - one
is located in Temecula, CA and one is located in Portland, OR.

As I use the tools available to help, my study would also help the
following target audience(s):

> 1.  Families with children
> 2.  Families with cultural backgrounds

The Foursquare API will enable me to research both dining establishments
as well as performing arts and other cultural facilities. I will review
the number of both as well as their proximity to my locations of choice.

> *Due to recent changes in the Foursquare API for security purposes, I
> will not dig into specific users and their comments or ratings.*

**Data**

Data for this study will be from multiple sources.

First, a collection of zip codes are downloaded from [US Zip Code
List](www.uszipcodelist.com) in comma separated values (CSV) format.
This is a comprehensive list that includes major city names, zip codes,
area codes, and the latitude and longitude of same.

Next, I will use the Foursquare API and Python to download venues, venue
categories, and other information related to the cities that I am
interested in. This information will complement the information from the
zip code list.

Finally, I will combine all of the above with my own prior knowledge of
these two locations. While data available online - particularly actual
reviews - are helpful, there is no substitute for "boots on the ground"
experience of going somewhere at least two or three times to understand
the neighborhood, the surroundings, and the availability of desired
goods and services.

**Methodology**

Using a Python notebook in Jupyter Labs, I first imported the zip code
data from the CSV file using Pandas to store it in a data frame. I used
Pandas sub-setting to further create two separate data frames, one for
each location of interest.

Using each location's data frame as a baseline, I used folium to first
plot maps of the locations. While maps can be very generic, one can get
a sense of the "busy-ness" of an area - how many cities are on the map
and how close are they to one another?

!\[Temecula,
CA\](<a href="https://github.com/NetGary0430/Coursera_Capstone/Temcula.png" class="uri">https://github.com/NetGary0430/Coursera_Capstone/blob/master/Temecula.png</a>)

!\[Portland,
OR\](<a href="https://github.com/NetGary0430/Coursera_Capstone/Portland.png" class="uri">https://github.com/NetGary0430/Coursera_Capstone/blob/master/Portland.png</a>)

I further used the data frames and the Foursquare API to download venue
information about each location. I used Python code to total up the
highest number of locations in the top 10 most common venues. That would
provide me additional information regarding my venues of choice - namely
food-related spots and cultural locations.

Moving beyond that, I then used additional Python code to further filter
the data by looking for areas that had my choice (restaurants and food
joints as well as museums and performing arts areas) within the first
*three* most common venues. This also enabled me to look at my locations
of choice and their surrounding areas to see if, for example, I might
live outside of a city proper, as one may work in a large city (e.g.
Chicago) but may live in a suburb (e.g. Schaumburg).

**Results**

Admittedly, I have traveled to my selected locations in prior business
travel. However, I did not realize how limited my knowledge of the
respective areas was. And I believed that I knew which location would
end up being my selection; however, once I reviewed the maps and the
data combined with my own experience, I stood corrected.

Temecula, CA is a larger city with a number of good dining choices. It
surprised me that, while Temecula proper has its share of good food,
there is a lot more retail and other establishments. I am an eater. I do
my shopping online (thank you, Amazon). Additionally I found that just
outside of Temecula, Riverside, actually had *more* dining options with
a mixture of both dine-in restaurants and smaller "joint" types of fast
food.

!\[Portland,
OR\](<a href="https://github.com/NetGary0430/Coursera_Capstone/Temecula_tbl.png" class="uri">https://github.com/NetGary0430/Coursera_Capstone/blob/master/Portland_tbl.PNG</a>)

Portland, OR, on the other hand, while having its fair share of dining
options, had fewer options than its more southern neighbor. I also
learned that Beaverton, OR would actually be a better choice for dining
than Portland proper. I should have been less surprised given the motto
to "Keep Portland Weird" - there were some areas where the most common
venue was a Tunnel, a carpet store, or a Yoga studio.

Certainly, those were *not* was I was interested in.

From a performing arts perspective, given the size of the Temecula area
versus that of Portland, I was not surprised that there were more
cultural-related venues such as museums and performing arts locations.

!\[Temecula,
OR\](<a href="https://github.com/NetGary0430/Coursera_Capstone/Portland_tbl.png" class="uri">https://github.com/NetGary0430/Coursera_Capstone/blob/master/Temecula_tbl.PNG</a>)

**Discussion**

While one may have visited an area - or even lived in an area - for a
long time, the ability to use tools such as the Foursquare API and the
Internet in conjunction with programming tools such as a Python Notebook
provides some enlightenment. I personally have lived in an area for
years and had someone take me to a restaurant that was literally 10
minutes from where I lived or worked but was completely unknown to me. I
received a shock anytime I asked, "How long have they been here" and the
answer was "23 years."

And I would love the place.

I do also note that, while I have a perception of what the area contains
regarding venues, looking at real data suggests that there are a lot
more *other* venues around that may slightly tweak my perception of that
area. What this does for anyone is plays into their preconceived notions
and biases of the type of people who frequent such venues. That also,
perhaps, taints their view of the area once they know the facts. Right,
wrong, or indifferent, we are humans.

I have often said, "In God we trust, all others bring good data."
Sometimes looking at the data will result in a change in heart. What was
once perceived to be "zigging" now becomes "zagging." An area one may
believe they will love may be overshadowed by an overwhelming amount of
evidence that another area is more attractive.

**Conclusion**

Based on what the data indicates, my "gut feel" that Portland would be
the winner was clearly wrong. As I researched the data - and followed up
with some additional online searching outside of the code - I found that
the outcome I expected was turned on its head. Not only are there more
numerous dining options in Riverside, CA, but they are also of the style
of food that I like. To me, as someone who spends a lot of time reading,
computing, and working with little time (or know-how) for cooking,
having that knowledge of an expansive availability of restaurants that I
would like in such a varying degree was reassuring.

My choice was to take the Temcula, CA position, but live outside of
Temecula in Riverside, CA.

