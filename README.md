#trick or track

##Intro: Tracking and HTTP requests

**In theory**, when we visit a website, our browser sends out data request frames in order to retrieve the information needed to render the page on our screen. **In reality**, request frames do not only serve the purpose of getting information, but also a way of identifying our computer. <br><br> **Here is an example:** Imagine a designer who wants to know how many people are visiting his website on a given day. For that, he uses Google Analytics, which means he adds a few lines of code into his website's source. Now, when we enter his domain into our browser and hit enter, communication between our computer and the router starts: We might get the HTML of his page first, then the images that are embedded, javascript files needed and, within it all, we send a request to that Google Analytics link in there, too. This happens all automatically. Google Analytics then sees that someone visited the website but also who (your device's MAC address). Google Analytics now knows *this* computer's user just visited *this* designer's website. Let's read the daily news now, maybe on nytimes.com - hello again Google Analytics, yes I am interested in design and think the New York Times writes good articles, add this to your profile. 

##Analysing: HTTP requests
This project is a Wifi Sniffer. It analyses HTTP request frames within a (insecure) wireless network by individual devices. The goal was to detect programatically which requests are the one's actually asked for, that is, the one's requesting information from the server that the domain entered into the browser points to, and which requests are a consequence of that, a chain reaction that takes place behind the scenes, without out awareness. <br> Here is a graph of the underlying assumptions of this program:





*process*