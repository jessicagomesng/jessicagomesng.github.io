---
layout: post
title:      "Rendering an Image at Mouse Position with React "
date:       2020-12-21 13:41:52 +0000
permalink:  rendering_an_image_at_mouse_position_with_react
---


I'm just about finished with my final project for Flatiron's Software Engineering Program, which involves creating an application using React! This has been very fun -- I actually really enjoy JavaScript and using React, and, although I've only just scratched the surface of using React to create programs, I'm really happy so far with the progress I've made! 

My application is an interactive experience where users view a map of Europe (I'd want to expand this to be global later!) and can 'click' on different countries to mark that they've visited them. Users can also leave 'pins' on the map with an image and caption to record different memories from their trips.

I wanted to find a way for a user to click on the map and drop a 'pin' at mouse position. At first, I tried implementing this with Canvas -- this was actually successful thanks to [this guide](https://medium.com/@pdx.lucasm/canvas-with-react-js-32e133c05258), but I found that it wasn't really what I needed. This is because objects on a canvas aren't actually associated with any data, and so, although I was able to render my pins where I wanted them to go, I couldn't use them to trigger any other events. Additionally, this allowed me to drop multiple markers on a map in one go, but I wanted a user to only create a marker once and then submit information about that marker to the database.

In the end, I found a much simpler solution to this! 

To implement this, I placed an event handler on my map, so that when clicked, the X and Y coordinates of the mouse could be recorded, eg:

```
handleClick(event) = {
this.setState({ showImage: true, 
xCoord: event.pageX,
yCoord: event.pageY )}
```

On click, the *showImage* attribute of state is set to true. This signals to the application to render an <img> of the marker on the page. In my render method, I have the following line:

```
                {this.state.showImage ? <img src={pin} style={{position: 'absolute', top: this.state.yCoord + 'px', left: this.state.xCoord + 'px'}} ref={this.markerRef} className="pin" alt="temporary pin"/> : null }
```

When showImage is set to true, then the image appears and a reference to it is established with *this.markerRef*. 

And...that's how I got it working! 

My next goal for my project is to take out any hardcoded styling -- eg right now, my map has defined width and height, which means that smaller window sizes or browsing on other devices (like a cell phone) would be fairly difficult.  I'll come back to how I accomplish this once I'm done...it's fairly involved at the moment! 
