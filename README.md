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
                console.log(date);
            }, // Callback to return the clicked date object
			year: "2012", // Optional start year, defaults to current year - pass in a year - Integer or String
			scroll_to_date: false // Scroll to the current day?
		});
	});
        
You'll have to source the calendar JS, the calendar CSS, and jQuery. The implementation is straight forward if you check out the example.

Have fun and please report any issues to the issue tracker here on GitHub.

~ JP

# License (MIT)

Copyright (C) 2012 John Patrick Given

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

