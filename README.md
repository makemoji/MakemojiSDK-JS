Makemoji SDK
====================

**Makemoji** is a free emoji keyboard for mobile apps. 

By installing our keyboard SDK every user of your app will instantly have access to new and trending emojis. Our goal is to increase user engagement as well as provide actionable real time data on sentiment (how users feel) and affinity (what users like). With this extensive data collection your per-user & company valuation will increase along with your user-base.
 
**Features Include**

* Extensive library of free emoji
* 722 standard Unicode emoji
* New emoji load dynamically
* Analytics Dashboard & CMS

To obtain your SDK key please email: sdk@makemoji.com

**[Learn More](http://makemoji.com/sdk)**


Setup
---------------------

* Using the Makemoji Javascript library requires the latest JQuery and Bootstrap libraries
	* [JQuery 2.x](https://code.jquery.com)
	* [Bootstrap](http://getbootstrap.com/2.3.2/)

* Add the following to your document head

```
<script src="https://d1tvcfe0bfyi6u.cloudfront.net/sdk/makemoji-1.2.min.js"></script>     
<link rel="stylesheet" type="text/css" href="https://d1tvcfe0bfyi6u.cloudfront.net/sdk/makemoji-1.2.min.css">
```

Usage
---------------------

On document ready, attach to a container where you want to display the text input.

```
    Makemoji.init('YOUR_SDK_KEY', "#container");

```

Only one instance of the Makemoji plugin can be used on a page.

To get the HTML output of the text input, trigger the getHTML() function.

```
    $('body').on('click', '#sendbutton', function(){
       var htmlOutput = Makemoji.getHTML();
   	 	// send to your back, display on page, etc
   	 });
       
```




FAQ
---------------------

*	The Makemoji SDK is completely free.

*	All emojis are served from AWS S3.

*	We do not store your messages. Your app backend will have to process and serve messages created with our SDK.

*	Your app's message volume does not affect the performance of our SDK.

*	Messages are composed of simple HTML containing image and paragraph tags. Formatting is presented as inline CSS.

Service Performance
---------------------

* Avg Service Repsonse Time: 100ms
 
* Hosted with AWS using Elastic Beanstalk & RDS

* Scales seamlessly to meet traffic demands
