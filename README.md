# jQuery Verbose Calendar

Why another jQuery calendar? I needed something very specific for a personal project which led me to created this calendar. After making it I thought it was pretty neat-o :)

Perhaps someone else will find it useful.

# Credit First

The plug-in makes use of Tipsy (http://onehackoranother.com) and jQuery.ScrollTo (http://flesler.blogspot.com/2007/10/jqueryscrollto.html).

If you already source these plugins, you'll want to remove them from the calendar plugin. I simply included them, with comments, to make the calendar implementation simpler.

# Implementation

    $(document).ready(function() {
    	$("#calendar-container").calendar({
			tipsy_gravity: 's', // How do you want to anchor the tipsy notification? (n / s / e / w)
			click_callback: function(date) {
                alert(date);
            }, // Callback to return the clicked date
			year: "2012", // Optional start year, defaults to current year - pass in a year - Integer or String
			scroll_to_date: false // Scroll to the current day?
		});
	});
        
You'll have to source the calendar JS, the calendar CSS, and jQuery. The implementation is straight forward if you check out the example.

Have fun and please report any issues to the issue tracker here on GitHub.

~ JP

