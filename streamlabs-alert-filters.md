# Hate Raid Filters for Streamlabs
These filters can prevent (some) malicious actors from triggering your Streamlabs alerts.

## Setup
Log into the Streamlabs Dashboard and go to your [Alertbox Settings](https://streamlabs.com/dashboard#/alertbox). Then scroll all the way down.
You will find an input box called ``Custom Bad Words``. Paste the first filter in there to block all of the terms and then hit the button called ``Blacklist``.
Alternatively, you can pick and choose from the individual filters below. Make sure not to accidentally include any extra spaces.

## All of the filters below in a single filter
(you do not need the others if you use this)

``regex:__$|(.)\1{4}|(?:^|[^g])r(?:a|4)p(?:e|3)|(?:0|o){2}3(?:1|i|l)|(?:0|o)3(?:1|i|l)[0-9]|(?:g|9)u(?:n|m)z(?:0|o)|(?:j|i){2}bu(?:i|1|l){2}d|(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)|(?:l|1|i)(?:a|4)r(?:s|5)h|(?:l|1|i)un(?:a|4)r|(?:n|m|r|1|l)(?:i|1|l|e)(?:g|9)+(?:(?:e|3|o|0)r|uh|a|4)|(?:o|0){2,}(?:l|i|1){2}(?:g|9)(?:a|4)n|(?:s|5)(?:i|1|l)m(?:o|0)+(?:l|i|1){2}|(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d|^gu[a-z]+da$|^gun[a-z][0-9]+$|b(?:a|4)b(?:o|0){2,}n|b(?:l|1|i)u(?:e|3)b(?:e|3)rr(?:y|i)d(?:o|0)g|d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|fr(?:i|1|l)(?:e|3)nd.*v(?:e|3)t(?:e|3)r(?:a|4)n|g(?:o|0)r(e|3)|h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n|h(?:a|4)t(?:e|3)|h(?:o|0)(?:s|5){2}|n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))|pt(?:s|5)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*fr(?:i|1|l)(?:e|3)nd|v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)``


## Filters based on structure
* **4+ consequent repeated letters**: ``regex:(.)\1{4}``
* **multiple underscores at end of name**: ``regex:__$``

## Filters based on common terms in hate raid accounts
* **0031**: ``regex:(?:0|o){2}3(?:1|i|l)``
* **031X**: ``regex:(?:0|o)3(?:1|i|l)[0-9]``
* **baboon**: ``regex:b(?:a|4)b(?:o|0){2,}n``
* **blueberrydog**: ``regex:b(?:l|1|i)u(?:e|3)b(?:e|3)rr(?:y|i)d(?:o|0)g``
* **dead...veteran**: ``regex:d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **died...veteran**: ``regex:d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **friend...veteran**: ``regex:fr(?:i|1|l)(?:e|3)nd.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **gore**: ``regex:g(?:o|0)r(?:e|3)``
* **gu...da**: ``regex:^gu[a-z]+da$``
* **gunxX**: ``regex:^gun[a-z][0-9]+$``
* **gunz0**: ``regex:(?:g|9)u(?:n|m)z(?:0|o)``
* **haha...veteran**: ``h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **hate**: ``regex:h(?:a|4)t(?:e|3)``
* **hoss**: ``regex:h(?:o|0)(?:s|5){2}``
* **jjbuild**: ``regex:(?:j|i){2}bu(?:i|1|l){2}d``
* **judgejudy**: ``regex:(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)``
* **larsh**: ``regex:(?:l|1|i)(?:a|4)r(?:s|5)h``
* **lunar**: ``regex:(?:l|1|i)un(?:a|4)r``
* **nigger and variants**: ``regex:(?:n|m|r|1|l)(?:i|1|l|e)(?:g|9)+(?:(?:e|3|o|0)r|uh|a|4)``
* **nigger (more variants)**: ``n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))``
* **ooligan**: ``regex:(?:o|0){2,}(?:l|i|1){2}(?:g|9)(?:a|4)n``
* **ptsd**: ``regex:pt(?:s|5)d``
* **rape (but not grape)**: ``regex:(?:^|[^g])r(?:a|4)p(?:e|3)``
* **simooli**: ``regex:(?:s|5)(?:i|1|l)m(?:o|0)+(?:l|i|1){2}``
* **suicid**: ``regex:(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d``
* **veteran...commit**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt``
* **veteran...dead**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d``
* **veteran...died**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d``
* **veteran...friend**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*fr(?:i|1|l)(?:e|3)nd``
* **veteran...haha**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)``
