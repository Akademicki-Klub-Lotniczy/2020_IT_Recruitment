# 2020 IT Recruitment


### Rules
* You have one month to complete a certain task (deadline: 20th of June)
* You can work on the task alone, or in groups of two
* During that month, you can contact us anytime, we'll be happy to answer any questions
* At the 20th of June, you will be presenting the results of your work, then we'll decide if you're good enough

### How to win?
It's not only about "doing a certain thing you're told to do".
Try to think forward, make suggestions on how a certain product/idea
you're working on could be developed further, tell us about the
observations you've made while working on your task.

We appreciate the people who explore the domain of the problem
they're working on, instead of just stratching
the surface to get a bare minimum - show us what you have done!

### The tasks

#

#### Web application, easy to use drone mission planner

Imagine you're working on a drone-based monitoring solution for
a company that builds railroad tracks. They want an easy-to-use
web application, that lets them plan missions for their monitoring
drones.

**Required features:**
* A map view (think [leaflet](https://leafletjs.com/))
* Ability to draw a map (preferably using markers)
* Ability to select a fragment of the path (between two markers), and change:
  - The speed at which the drone should fly on this fragment
  - Whether or not the drone should take pictures while on this fragment
* Ability to save and load the created mission to/from a JSON string

**Nice to have features:**
* Usage of a modern web framework (show us what you can do)
* Nice UX

#

#### A library to convert between Geographic and carthesian coordinates

It's way easier to think and build algorithms, that operate on carthesian 
coordinate system. Unfortunately, drones and planes only operate
on geographic coordinates (since they use GPS), which makes it hard to 
write code that tells, whether a drone is inside a certain square or has
crossed a certain line, drawn on the ground (such operations are
often required on competitions, for stuff like precision landing).

Note that those tasks would be trivial, if we used a carthesian coordinate
system. That's why we need a converter.

**Requirements:**
* Being able to draw basic geometric objects (say, squares, lines, circles) in a carthesian coordinate system (i will refer to this environment as "the map")
* Being able to set how the map translates to the real (GPS-coords based) world, by setting an origin point, and the map's rotation
* Having provided a certain point in GPS coordinates, the library should tell us whether it intersects with the squares and circles on the map, how close it is to the lines we've drawn on the map

**Nice to have features**:
- Visualisation of the map 
- A GUI to draw on the map

#

#### GTA V scripting/environment modeling (for real, this is not a joke)

We need training data for neural networks, and it turns out,
that they work surprisingly good on the datasets made in GTA V.

We need a dataset consisting of pictures of roads, filled with cars,
taken from the height of 10-30 meters. Like [this picture](road.jpg)

#

#### A web application for streaming and processing video

Let's say we have a drone with a camera, and an internet connection. We want to stream
the video from the drone (You can simply use a Raspberry Pi with any camera) to a web server.

The server will then:
- Allow us to watch the incoming stream from a web page
- Save the incoming stream to a file

Think [video.js](https://videojs.com/), [ffmpeg](https://www.ffmpeg.org/), [webrtc](https://www.html5rocks.com/en/tutorials/webrtc/basics/)

**Requirements**
- At least 480p, fluid video stream
- Doesn't have to work on mobile, but has to work on a desktop browser
