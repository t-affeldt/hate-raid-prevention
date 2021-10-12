# Hate Raid Filters for StreamElements
These filters can be used to completely ban (some) malicious accounts on sight.
StreamElements does not have a filter system for their alerts but a general content-moderation filter. Thus, this list is much shorter than the one for Streamlabs because false-positives will have a much greater impact.
If one of your viewers gets wrongfully banned, you will have to mark them as a ``Regular`` and unban them.

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
(you do not the individual filters if you use this)

``(?:^|[^g])r(?:a|4)p(?:e|3)|(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d|b(?:a|4)b(?:o|0){2,}n|g(?:o|0)r(e|3)|h(?:a|4)t(?:e|3).*r(?:a|4)(?:i|1|l)d|pt(?:s|5)d|h(i|1|l)t(?:l|i|1)(?:e|3)r|(?:n|r|1|l)(?:i|1|l)(?:g|9){2,}(?:(?:e|3|o|0)r|uh|a|4)|n(?:e|3)(?:g|9)+(?:(?:e|3|o|0)r|uh|(?:a|4)(?:[^a-z]|$))|n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))|d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n|v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)|h(?:o|0)(?:s|5){2}|(?:0|o){2}3(?:1|i|l)|(?:0|o)3(?:1|i|l)[0-9]|(?:g|9)u(?:n|m)z(?:0|o)|(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)|(?:l|1|i)(?:a|4)r(?:s|5)h|k(?:i|1|l){3}.*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*k(?:i|1|l){3}|(?:g|9)(?:a|4)(?:s|5).*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*(?:g|9)(?:a|4)(?:s|5)|murd(?:e|3)r.*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*murd(?:e|3)r|dr(?:o|0)wn.*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*dr(?:o|0)wn|(?:g|9)(?:a|4)(?:s|5).*ch(?:a|4)mb(?:e|3)r|k(?:i|1|l){3}.*(?:g|9)(?:a|4)(?:y|i)|(?:g|9)(?:a|4)(?:y|i).*k(?:i|1|l){3}|(?:g|9)(?:a|4)(?:s|5).*(?:g|9)(?:a|4)(?:y|i)|(?:g|9)(?:a|4)(?:y|i).*(?:g|9)(?:a|4)(?:s|5)|murd(?:e|3)r.*(?:g|9)(?:a|4)(?:y|i)|(?:g|9)(?:a|4)(?:y|i).*murd(?:e|3)r|dr(?:o|0)wn.*(?:g|9)(?:a|4)(?:y|i)w|(?:g|9)(?:a|4)(?:y|i).*dr(?:o|0)wn|^gun[a-z][0-9]+$``

## Individual filters
You do not need these if you use the one above.
Pick and choose from these filters if the one on top is too strict for you.

### Impersonated account names
* **0031**: ``(?:0|o){2}3(?:1|i|l)``
* **031X**: ``(?:0|o)3(?:1|i|l)[0-9]``
* **gunz0**: ``(?:g|9)u(?:n|m)z(?:0|o)``
* **hoss**: ``h(?:o|0)(?:s|5){2}``
* **judgejudy**: ``(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)``
* **larsh**: ``(?:l|1|i)(?:a|4)r(?:s|5)h``

### Bad terms
* **baboon**: ``b(?:a|4)b(?:o|0){2,}n``
* **gore**: ``g(?:o|0)r(?:e|3)``
* **gunxX**: ``^gun[a-z][0-9]+$``
* **hate...raid**: ``h(?:a|4)t(?:e|3).*r(?:a|4)(?:i|1|l)d``
* **hitler**: ``h(i|1|l)t(?:l|i|1)(?:e|3)r``
* **ptsd**: ``pt(?:s|5)d``
* **rape (but not grape)**: ``(?:^|[^g])r(?:a|4)p(?:e|3)``
* **suicid**: ``(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d``

### Hate Speech against People of Color
* **nigger and variants (1/3)**: ``(?:n|r|1|l)(?:i|1|l)(?:g|9){2,}(?:(?:e|3|o|0)r|uh|a|4)``
* **nigger and variants (2/3)**: ``n(?:e|3)(?:g|9)+(?:(?:e|3|o|0)r|uh|(?:a|4)(?:[^a-z]|$))``
* **nigger and variants (3/3)**: ``n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))``

### Hate Speech against LGBTQIA+
* **drown...gay**: ``dr(?:o|0)wn.*(?:g|9)(?:a|4)(?:y|i)w``
* **gas...gay**: ``(?:g|9)(?:a|4)(?:s|5).*(?:g|9)(?:a|4)(?:y|i)``
* **gay...drown**: ``(?:g|9)(?:a|4)(?:y|i).*dr(?:o|0)wn``
* **gay...gas**: ``(?:g|9)(?:a|4)(?:y|i).*(?:g|9)(?:a|4)(?:s|5)``
* **gay...kill**: ``(?:g|9)(?:a|4)(?:y|i).*k(?:i|1|l){3}``
* **gay...murder**: ``(?:g|9)(?:a|4)(?:y|i).*murd(?:e|3)r``
* **kill...gay**: ``k(?:i|1|l){3}.*(?:g|9)(?:a|4)(?:y|i)``
* **murder...gay**: ``murd(?:e|3)r.*(?:g|9)(?:a|4)(?:y|i)``

### Hate Speech against Religious Groups
* **drown...jew**: ``dr(?:o|0)wn.*(?:j|i)(?:e|3)w``
* **gas...chamber**: ``(?:g|9)(?:a|4)(?:s|5).*ch(?:a|4)mb(?:e|3)r``
* **gas...jew**: ``(?:g|9)(?:a|4)(?:s|5).*(?:j|i)(?:e|3)w``
* **jew...drown**: ``(?:j|i)(?:e|3)w.*dr(?:o|0)wn``
* **jew...gas**: ``(?:j|i)(?:e|3)w.*(?:g|9)(?:a|4)(?:s|5)``
* **jew...kill**: ``(?:j|i)(?:e|3)w.*k(?:i|1|l){3}``
* **jew...murder**: ``(?:j|i)(?:e|3)w.*murd(?:e|3)r``
* **kill...jew**: ``k(?:i|1|l){3}.*(?:j|i)(?:e|3)w``
* **murder...jew**: ``murd(?:e|3)r.*(?:j|i)(?:e|3)w``

### Hate Speech against Veterans
* **dead...veteran**: ``d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **died...veteran**: ``d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **veteran...commit**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt``
* **veteran...dead**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d``
* **veteran...died**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d``
* **veteran...haha**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)``
* **haha...veteran**: ``h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n``

## Optional (strict) filters
These are the remaining filters from the Streamlabs filter list.
They are not included in the condensed filter on the top.
You can enable them for extra security but it is possible that they will also ban some non-malicious viewers. I recommend to instead use only the filters above and install a moderation bot like [Smashbot](https://www.smashbot.live).

* **4+ consequent repeated letters**: ``(.)\1{4}``
* **4+ consequent identical looking characters**: ``(?:i|1|l){4}|(?:e|3){4}|(?:o|0){4}|(?:s|5){4}``
* **multiple underscores at end of name (against impersonation)**: ``__$``
* **7+ consequent numbers (against phone number doxxing)**: ``[\d|_]{7}``
* **blueberrydog**: ``b(?:l|1|i)u(?:e|3)b(?:e|3)rr(?:y|i)d(?:o|0)g``
* **friend...veteran**: ``fr(?:i|1|l)(?:e|3)nd.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **gu...da**: ``^gu[a-z]+da$``
* **hate**: ``h(?:a|4)t(?:e|3)``
* **jjbuild**: ``(?:j|i){2}bu(?:i|1|l){2}d``
* **lunar**: ``(?:l|1|i)un(?:a|4)r``
* **ooligan**: ``(?:o|0){2,}(?:l|i|1){2}(?:g|9)(?:a|4)n``
* **simooli**: ``(?:s|5)(?:i|1|l)m(?:o|0)+(?:l|i|1){2}``
* **veteran...friend**: ``v(?:e|3)t(?:e|3)r(?:a|4)n.*fr(?:i|1|l)(?:e|3)nd``
