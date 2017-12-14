### Purpose

There are many great online tools for converting between timezones.

Wouldn't it be great to have a tool that spits out what time it is in **all** the **timezones you care about** at once? Or what time it will be in Singapore when it is 9pm on Monday in Atlanta? Without any complicated syntax to memorize or waiting for your browser to load?

### Installation

Download the `whenisit` script. Open it in a text editor.

Edit the four variables at the top. Instructions are in the file. If you don't know your timezone, web search "iana timezone MY CITY". If the positional arrays don't make sense to you, simply uncomment the examples and run `whenisit`. Things will be clearer.

Save the file.

Optionally, move it to somewhere in your path like `/usr/local/bin/`.

### How to use this script

1. What time is it now? (This uses your personal list of timezones.)

        $ whenisit

  Sample output:

        02:34 Thu, Dec 14 -- UTC
        02:34 Thu, Dec 14 -- ranger, nightwatchman
        03:34 Thu, Dec 14 -- witch
        21:34 Wed, Dec 13 -- beatbox, rando, egghead
        18:34 Wed, Dec 13 -- pidg

2. What time is it later?

        $ whenisit 6 pm

  What about the daylight savings time thing later this week?
  
        $ whenisit 11am sat

3. What time is it around the globe?

        $ whenisit -a
        
  or
        $ whenisit -a March 16 8pm

  Sample output:
  
        . . .
        06:23 Wed, Dec 13 -- America/Caracas
        07:23 Wed, Dec 13 -- America/Santiago
        06:53 Wed, Dec 13 -- America/St_Johns
        . . .
        13:53 Wed, Dec 13 -- Asia/Tehran
        14:23 Wed, Dec 13 -- Asia/Baku
        14:53 Wed, Dec 13 -- Asia/Kabul
        . . .

4. What time is it in Helsinki?

        $ whenisit -aa | grep Helsinki

  in Louisville?
  
        $ whenisit -aa | grep Loui

And that's it! :) See any improvements, submit a PR.
