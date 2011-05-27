**Note:** This is now deprecated in favor of sinatra-support. See:

 * http://sinefunc.com/sinatra-support (Sinatra::UserAgentHelpers)
 * http://github.com/sinefunc/sinatra-support

Agent sniff
===========

Usage example:

    Main.register Sinatra::UserAgentHelpers
   
    -# haml
    %body{class: browser.body_class}
   
    - if browser.ios?
      %p Download our mobile app!

Possible outputs:

    <body class='webkit safari mac'>
    <body class='windows ie ie6'>

More stuff:

    browser.webkit?
    browser.android?
    browser.gecko?
    browser.ie8?
    # and many more!
