##QuickAccord##
*By: AJ Savino*

QuickAccord - A simple jQuery accordion plugin. Supports IE8, accessibility standards, and CSS3 transitions.

###Implementation###
Include JS on your page in addition to jQuery. Modify the CSS to fit your needs.

HTML
```html
<!-- You can add class "collapsed" or "expanded" to change the default state -->
<!-- 'data-accord-group' attribute is optional -->
<ul>
	<li>
		<a href="#accordion1" class="accordion-trigger" data-accord-group="group1">Accordion 1</a>
		<div id="accordion1" class="accordion-content collapsed">
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In non nisi et nulla vehicula cursus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas id arcu at purus imperdiet aliquam. Cras lacinia faucibus ligula, id lacinia turpis lobortis quis. Maecenas non accumsan massa. Cras et malesuada magna, porta tempor sem. Maecenas pellentesque consequat dolor ac lobortis. Ut sed ipsum iaculis neque pretium eleifend. Suspendisse lacus nisi, fermentum non turpis ut, iaculis efficitur purus. Phasellus tristique et nisl et cursus. Ut felis metus, cursus eu blandit a, imperdiet a odio. Donec posuere ut lectus eget semper. Aenean sed sem consectetur, venenatis magna eget, egestas lorem. Proin rutrum ac nunc sed laoreet. Aenean efficitur lacus turpis, vel facilisis tellus efficitur in.</p>
		</div>
	</li>
	<li>
		<a href="#accordion2" class="accordion-trigger" data-accord-group="group1">Accordion 2</a>
		<div id="accordion2" class="accordion-content collapsed">
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In non nisi et nulla vehicula cursus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas id arcu at purus imperdiet aliquam. Cras lacinia faucibus ligula, id lacinia turpis lobortis quis. Maecenas non accumsan massa. Cras et malesuada magna, porta tempor sem. Maecenas pellentesque consequat dolor ac lobortis. Ut sed ipsum iaculis neque pretium eleifend. Suspendisse lacus nisi, fermentum non turpis ut, iaculis efficitur purus. Phasellus tristique et nisl et cursus. Ut felis metus, cursus eu blandit a, imperdiet a odio. Donec posuere ut lectus eget semper. Aenean sed sem consectetur, venenatis magna eget, egestas lorem. Proin rutrum ac nunc sed laoreet. Aenean efficitur lacus turpis, vel facilisis tellus efficitur in.</p>
		</div>
	</li>
	<li>
		<a href="#accordion3" class="accordion-trigger" data-accord-group="group1">Accordion 3</a>
		<div id="accordion3" class="accordion-content collapsed">
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In non nisi et nulla vehicula cursus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas id arcu at purus imperdiet aliquam. Cras lacinia faucibus ligula, id lacinia turpis lobortis quis. Maecenas non accumsan massa. Cras et malesuada magna, porta tempor sem. Maecenas pellentesque consequat dolor ac lobortis. Ut sed ipsum iaculis neque pretium eleifend. Suspendisse lacus nisi, fermentum non turpis ut, iaculis efficitur purus. Phasellus tristique et nisl et cursus. Ut felis metus, cursus eu blandit a, imperdiet a odio. Donec posuere ut lectus eget semper. Aenean sed sem consectetur, venenatis magna eget, egestas lorem. Proin rutrum ac nunc sed laoreet. Aenean efficitur lacus turpis, vel facilisis tellus efficitur in.</p>
		</div>
	</li>
</ul>
```

JS
```html
$(".accordion-trigger").QuickAccord();
```

----------

####JavaScript API####
```javascript
/* Methods */

var qa = $(".accordion-trigger").QuickAccord();

//Called automatically
qa.QuickAccord.init();

//Destroys the QuickAccord instance and will need to be reinitialized
qa.QuickAccord.destroy();

//Collapses / Expands the accordion content
qa.QuickAccord.toggle();

//Collapses the accordion content
qa.QuickAccord.collapse();

//Expands the accordion content
qa.QuickAccord.expand();

//Returns true if the accordion content is expanded
qa.QuickAccord.isExpanded();
```