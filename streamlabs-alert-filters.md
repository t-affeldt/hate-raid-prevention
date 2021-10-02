# Hate Raid Filters for Streamlabs
These filters can prevent (some) malicious actors from triggering your Streamlabs alerts.
Go to your [Alertbox Settings](https://streamlabs.com/dashboard#/alertbox) and scroll all the way down.
You will find an input box called ``Custom Bad Words``. Paste the first filter in there to block all of the terms and then hit the button called ``Blacklist``.
Alternatively, you can pick and choose from the individual filters below. Make sure not to accidentally include any extra spaces.

All of the filters below in a single filter
=======================================
(you do not need the others if you use this)

``regex:__$|(.)\1{4}|(?:^|[^g])r(?:a|4)p(?:e|3)|(?:0|o){2}3(?:1|i|l)|(?:0|o)3(?:1|i|l)2|(?:g|9)u(?:n|m)z(?:0|o)|(?:j|i){2}bu(?:i|1|l){2}d|(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)|(?:l|1|i)un(?:a|4)r|(?:n|m|r|1|l)(?:i|1|l)(?:g|9){2,}(?:er|3r|a|4)|(?:o|0){2,}(?:l|i|1){2}(?:g|9)(?:a|4)n|(?:s|5)(?:i|1|l)m(?:o|0)+(?:l|i|1){2}|(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d|b(?:a|4)b(?:o|0){2,}n|b(?:l|1|i)u(?:e|3)b(?:e|3)rr(?:y|i)d(?:o|0)gs|d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|fr(?:i|1|l)(?:e|3)nd.*v(?:e|3)t(?:e|3)r(?:a|4)n|h(?:a|4)t(?:e|3)|h(?:o|0)(?:s|5){2}|pt(?:s|5)d.*tr(?:i|1|l)(?:g|9){2,}(?:e|3)r|tr(?:i|1|l)(?:g|9){2,}(?:e|3)r.*pt(?:s|5)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*fr(?:i|1|l)(?:e|3)nd``


Filters based on structure:
=====================================
* **multiple underscores at end of name**: ``regex:__$``
* **4+ consequent repeated letters**: ``regex:(.)\1{4}``

Filters based on common terms in hate raid accounts:
=======================================
* **rape (but not grape)**: ``regex:(?:^|[^g])r(?:a|4)p(?:e|3)``
* **0031**: ``regex:(?:0|o){2}3(?:1|i|l)``
* **0312**: ``regex:(?:0|o)3(?:1|i|l)2``
* **gunz0**: ``regex:(?:g|9)u(?:n|m)z(?:0|o)``
* **jjbuild**: ``regex:(?:j|i){2}bu(?:i|1|l){2}d``
* **judgejudy**: ``regex:(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)``
* **lunar**: ``regex:(?:l|1|i)un(?:a|4)r``
* **nigger and variants**: ``regex:(?:n|m|r|1|l)(?:i|1|l)(?:g|9){2,}(?:er|3r|a|4)``
* **ooligan**: ``regex:(?:o|0){2,}(?:l|i|1){2}(?:g|9)(?:a|4)n``
* **simooli**: ``regex:(?:s|5)(?:i|1|l)m(?:o|0)+(?:l|i|1){2}``
* **suicid**: ``regex:(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d``
* **baboon**: ``regex:b(?:a|4)b(?:o|0){2,}n``
* **blueberrydogs**: ``regex:b(?:l|1|i)u(?:e|3)b(?:e|3)rr(?:y|i)d(?:o|0)gs``
* **dead...veteran**: ``regex:d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **died...veteran**: ``regex:d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **friend...veteran**: ``regex:fr(?:i|1|l)(?:e|3)nd.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **hate**: ``regex:h(?:a|4)t(?:e|3)``
* **hoss**: ``regex:h(?:o|0)(?:s|5){2}``
* **ptsd...trigger**: ``regex:pt(?:s|5)d.*tr(?:i|1|l)(?:g|9){2,}(?:e|3)r``
* **trigger...ptsd**: ``regex:tr(?:i|1|l)(?:g|9){2,}(?:e|3)r.*pt(?:s|5)d``
* **veteran...commit**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt``
* **veteran...dead**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d``
* **veteran...died**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d``
* **veteran...friend**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*fr(?:i|1|l)(?:e|3)nd``
