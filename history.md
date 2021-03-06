

![React_banner](/images/react_banner.png)

# The History of React.

ReactJS started out as a library for [XHP](https://web.facebook.com/notes/facebook-engineering/xhp-a-new-way-to-write-php/294003943919/?_rdc=1&_rdr). XHP is [Facebook's](https://www.facebook.com) version of [PHP](http://php.net/manual/en/intro-whatis.php), which was open-sourced in 2010. The aim of creating XHP was to make frontend development easier and help avoid cross-site scripting attacks (XSS). XSS is a very common attack vector that inserts malicious codes into a web application. 

XSS does not attack the web application directly, instead, it attacks the users of such web applications by attaching an embedded javascript code to the user's request which in turn steals information and compromises the integrity of the user trying to access a resource on a web application. 

This is where XHP comes in, XHP has an **Automatic XSS protection**;  all page rendering is done inside XHP and it knows what an Hypertext Markup Language (HTML) is and what a context is, hence escaping all contexts without any hassle. 

However, XHP failed when it comes to building dynamic web applications. Meaning, once a change occurs, or a state changes, the web application rerenders itself, causing the user to lose any information previously stored in the [Document Object Model](https://www.w3.org/TR/DOM-Level-2-Core/introduction.html) (DOM). This got Facebook Ads Org team thinking, why do we have to rerender the entire page just because a state changed?. They realized early enough that this process was terrible for Performance as well as User Experience. 

In the year 2011, [Jordan Walke](https://twitter.com/jordwalke), a Software developer at Facebook, started working on a prototype to make this process more efficient while providing a reasonable user experience too. And this was how a JavaScript library for building user interfaces was conceived (React).  Few months after, The Like and commenting features on Facebook site were built using React and [Flux](https://facebook.github.io/flux/).

Now, around this same time when Facebook started using React on the like and commenting UI, and also on the Ads product (2012); [Instagram](https://www.instagram.com/) joined Facebook. One of the first products they wanted to build was their [website](https://www.instagram.com/). After taking a good look at facebook's stack,  [Pete Hunt](https://twitter.com/floydophone) made a case to use React on Instagram's website. But at the time, React was closely coupled to facebook's stack. Pete Hunt did not give up, he did most of the work required to decouple React from Facebook's stack so that Instagram could use React as well; thereby making Instagram the first external product to use React. With this, Facebook was a step away to blessing developers around the world with the awesomeness of React.

May 2013, React was open-sourced at JSConf in the United States. And from then till now, many developers across the world actively use React in production. Companies like, Trello, Slack, Docker, Airbnb, Khan Academy, New York Times, Codecademy to mention a few actively use React.

In April 2015, Facebook released a patent as regards the usage of React; Which basically says, "In as much as you do not sue us for patent infringement, we will give you this software for free; you can sell, distribute, import, make, and use this product. In addition, we also promise not to sue you for any patent infringement as regards this open source software". You can read about it [here](https://github.com/facebook/react/blob/master/PATENTS). 

#### 5 Highlights of React?

1. **Virtual Document Object Model:** To explain this, Let us picture a "Car" object, with 4 wheels, 4 doors, colored black, let us give it a name of "Pusher". When there is a change in any of this properties; say, the color was changed to "matte black". What React does, is to perform a "diffing algorithm", which essentially mean to identify what has changed. Once it notices the change, it then performs another step called "reconciliation", which essentially updates the DOM with the result of diffing algorithm .isn't that cool?. Instead of updating the entire DOM, it is smart enough to update just the nodes that changed.
2. **Server- Side Rendering:**  Because React can comfortably handle server-side rendering; when a user makes a request to our application, the server renders and packages as an HTML string; the required components needed for our application to show up, after which it sends the response to the client. Once the components get to the client, the client renders the page. 
3. **React Native:** [React Native](https://facebook.github.io/React-native/) was released in 2015, The Library allows developers build real ***native*** Andriod and iOS applications using javascript and React. In effect, learning Java and Objective-C is no longer a requirement for building ***native*** applications. 
4. **React VR:** At the just concluded [F8 Developer Conference](https://www.fbf8.com/), [React VR](https://facebook.github.io/React-vr/) was released to the public. React VR allows developers create Virtual reality (VR) applications using only Javascript. React VR also leverages on [WebGL](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API) and [WebVR](https://webvr.info/) to bring the perfect VR experience to the user. Just like React, Developers can now create awesome VR experiences by using the declarative components approach.
5. **React Fiber:** React Fiber, also know as React 16, was *introduced* to the public at React Conf 2017, It promises to be a complete reimplementation of the React core algorithm from the ground up, with support for built-in scheduling and incremental rendering. It is an update that is fully backward compatible with existing applications made with React. React Fiber is not yet ready for public consumption, but you can visit this [link](http://isfiberreadyyet.com/) to follow up with the release.

  ​

Thanks for reading!.