---
layout: modules
title: Mobify.js Carousel Module
---

<link rel="stylesheet" href="{{ site.baseurl }}/static/examples/css/accordion.css">
<link rel="stylesheet" href="{{ site.baseurl }}/static/examples/css/accordion-controls.css">

# Accordion

Try it out:

<ul class="m-accordion">
    <li class="m-item">
        <h3 class="header">
            <a>Tab1</a>
        </h3>
        <div class="content">
            <div class="inner-content">
                <h2>Content 1</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui icia deserunt mollit anim id est laborum.</p>
            </div>
        </div>
    </li>
    <li class="m-item">
        <h3 class="header">
            <a>Tab2</a>
        </h3>
        <div class="content">
            <div class="inner-content">
                <h2>Content 2</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p> 
            </div>
        </div>
    </li>
    <li class="m-item">
        <h3 class="header">
            <a>Tab3</a>
        </h3>
        <div class="content">
            <div class="inner-content">
                <h2>Content 3</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui icia deserunt mollit anim id est laborum.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui icia deserunt mollit anim id est laborum.</p>
            </div>
        </div>
    </li>
</ul>

<div class="btn-container">
	<a href="{{ site.baseurl }}/modules/accordion-examples" class="btn btn-primary">Download Accordion</a>
	<a href="{{ site.baseurl }}/modules/accordion-examples" class="see-examples">See more examples</a>
</div>

## Using mobify-accordion.js

To initialize an accordion, use the markup documented below, and call the jQuery/Zepto initializer.

	$('.m-accordion').accordion()

## Markup

The basic markup is composed out of a ul `.m-accordion`, and numerous lis `m-item`. Each `m-item` contains a
h3 `header` where the title of the item goes, and a div `content`, which contains a div `inner-content` which
must contain the content for the item.

	<ul class="m-accordion">
	    <li class="m-item">
	        <h3 class="header">
	            <a>Tab1</a>
	        </h3>
	        <div class="content">
	            <div class="inner-content">
	                <h2>Content 1</h2>
	                <h2>Lorem Ipsum</h2>
	            </div>
	        </div>
	    </li>
	    <li class="m-item">
	        <h3 class="header">
	            <a>Tab2</a>
	        </h3>
	        <div class="content">
	            <div class="inner-content">
	                <h2>Content 2</h2>
	                <p>Lorem Ipsum</p>
	            </div>
	        </div>
	    </li>
	    <li class="m-item">
	        <h3 class="header">
	            <a>Tab3</a>
	        </h3>
	        <div class="content">
	            <div class="inner-content">
	                <h2>Content 3</h2>
	                <p>Lorem Ipsum</p>
	            </div>
	        </div>
	    </li>
	</ul>

## Methods

### .accordion(options)

Initializes the accordion.

    $('.m-accordion').carousel();

### .accordion('unbind')

Removes any tap, mouse, and other event handlers from the accordion.

    $('.m-accordion').accordion('unbind');

### .accordion('bind')

Restores the tap, mouse, and other event handlers for the accordion.

    $('.m-accordion').accordion('bind');

### .accordion('destroy')

Unbinds the events from the accordion, and removes it from the DOM.

    $('.m-accordion').accordion('destroy');

<script src="{{ site.baseurl }}/static/examples/js/accordion.js"></script>
<script>
    $(function() { $('.m-accordion').accordion(); });
</script>