Lil.js: Keeping it simple (and Lil)
===================================

*Lil.js* is a Lil JavaScript library for people who want to KISS (Keep It Simple, Stupid) and keep their imports under 1KB. The syntax is similar to jQuery's (though I have NO affiliation with them) so you can switch over to jQuery if you feel the need with minimal code changes.

Installation
------------
If you don't know how to work with a JS file, go use the Google machine.

Usage
-----
The basic selector is easy to work with. Just pass it a string containing the ID you want to get.

    $("idOfTarget");

That isn't very useful though, so you can specify an event listener with the "on" function.

    $("idOfTarget").on("click", function() { var x=1; doStuff(x); });
    $("idOfTarget").on("keyup", function() { var x=1; doStuff(x); });

You can use any valid JavaScript event as the first parameter to "on", and just pass a function as the second parameter.

If you need a raw reference to the item, simply use the "raw" function.

    $("idOfTarget").raw().checked = true;

This gives you the same result as:

    document.getElementById("idOfTarget").checked = true;

but it's shorter and less of a pain to type.

Notes
-----
- There's very little implemented right now, but I'll expand it over time.
- If you have a request, send me a message here on GitHub.
- Once the fully expanded file reaches a certain size, I'll provide a condensed version too.

