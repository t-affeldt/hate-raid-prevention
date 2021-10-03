# Hate Raid Filters for StreamElements
These filters can be used to completely ban (some) malicious accounts on sight.
StreamElements does not have a filter system for their alerts but a general content-moderation filter. Thus, this list is much shorter than the one for Streamlabs because false-positives will have a much greater impact.
If one of your viewers gets wrongfully banned, there is no way of unbanning them again without completely disabling the respective filter. Use at your own risk.

## Setup
1) Log into the StreamElements dashboard.
2) Go to your [Spam Filter Settings](https://streamelements.com/dashboard/bot/spam-filters).
3) Make sure that ``Banned Words`` filter is enabled.
4) Click on ``Edit``.
5) Click ``Create New Group``.
6) Enter anything of your choice into ``Group Name`` (like ``Account Name Filters``).
7) Turn on the filter.
8) Untick the check box called ``Messages`` under ``Scan Section``. Make sure that ``Username`` remains turned on.
9) Click ``Add New Banned Phrase``.
10) Copy the first filter on this list into the text input called ``Enter banned phrase``.
11) Tick the check box next to the text input that says ``Regular expression``.
12) Click the button called ``Save`` next to the check box.
13) Click ``Test Filters``.
14) Enter ``gunp0`` as ``Username`` and hit ``Test``.
15) If you have done everything correctly, it should say ``Phrase matches: Account Name Filters``.

Alternatively, you can also pick and choose from the list of filters.
Create a new banned phrase for each one and then copy the respective filter into the text input. Make sure to enable ``Regular expression`` for every one of them.

## All of the filters below in a single filter
(you do not the others if you use this)

``b(?:a|4)b(?:o|0){2,}n|d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|g(?:o|0)r(e|3)|^gun[a-z][0-9]+$|h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n|(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)|(?:l|1|i)(?:a|4)r(?:|5)h|(?:n|m|r|1|l)(?:i|1|l|e)(?:g|9)+(?:(?:e|3|o|0)r|uh|a|4)|n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))|pt(?:s|5)d|(?:^|[^g])r(?:a|4)p(?:e|3)|(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)``

# Individual filters based on terms in hate raid accounts
* **baboon**: ``b(?:a|4)b(?:o|0){2,}n``
* **dead...veteran**: ``d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **died...veteran**: ``d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **gore**: ``g(?:o|0)r(?:e|3)``
* **gunxX**: ``^gun[a-z][0-9]+$``
* **haha...veteran**: ``h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **judgejudy**: ``(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)``
* **larsh**: ``(?:l|1|i)(?:a|4)r(?:s|5)h``
* **nigger and variants**: ``(?:n|m|r|1|l)(?:i|1|l|e)(?:g|9)+(?:(?:e|3|o|0)r|uh|a|4)``
* **nigger (more variants)**: ``n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))``
* **ptsd**: ``pt(?:s|5)d``
* **rape (but not grape)**: ``(?:^|[^g])r(?:a|4)p(?:e|3)``
* **suicid**: ``(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d``
* **veteran...commit**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt``
* **veteran...dead**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d``
* **veteran...died**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d``
* **veteran...haha**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)``