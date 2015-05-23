# ASCII Art in your Salesforce Debug Log

Believe it or not this silly thing came about as a result of a real project. 

More about that soon. 

But basically, I was asked to put something in the debug log that could not be missed amongst all other messages. Someone on the team showed me the [Text-to-ASCII-art generator][1] on patorjk.com. 

Initially, I just copy-pasted the text generated, added some new-line characters, got my log message in there, and it was all good. 

And then [CodeFriar noticed][2] and wanted to see the code. 

My first response was, "what code?" 

Who cares about a silly little single debug statement with a whole lot of text in it. 

Of course then, the lightbulb went on...the world needs text-to-ASCII log messages. They really do. 

So this is the work in progress. 

##Status

###Done
- Using [4max][3] font ASCII characters from [patorjk.com][4]
- Made slight adjustments to get rid of double quote characters and escape single quotes
- Have basic "write to log" functionality working
- Supporting characters [SPACE], 0-9, A-Z (upper only)

###Planned
- Move character dictionary to custom metadata type
- Add Visualforce UI so non-Coders can join in the fun
- Validate/ToUpper the text entry
- Limit length of entry (truncate? throw exception?)
- Extend dictionary to support some punctuation and lowercase
- Create managed package for demo of custom metadata type

[1]: http://patorjk.com/software/taag
[2]: https://twitter.com/codefriar/status/601454449907793920
[3]: http://patorjk.com/software/taag/#p=display&f=4Max&t=1%202%203%204%205%206%207%208%209%200%20A%20B%20C%20D%20E%20F%20G%20H%20I%20J%20K%20L%20M%20N%20O%20P%20Q%20R%20S%20T%20U%20V%20W%20X%20Y%20Z
[4]: http://patorjk.com