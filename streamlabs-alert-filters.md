# Hate Raid Filters for Streamlabs
These filters can prevent (some) malicious actors from triggering your Streamlabs alerts.

## Setup
Log into the Streamlabs Dashboard and go to your [Alertbox Settings](https://streamlabs.com/dashboard#/alertbox). Then scroll all the way down.
You will find an input box called ``Custom Bad Words``. Paste the first filter in there to block all of the terms and then hit the button called ``Blacklist``.
Alternatively, you can pick and choose from the individual filters below. Make sure not to accidentally include any extra spaces.

## All of the filters below in a single filter
(you do not need the others if you use this)

``regex:__$|(.)\1{4}|(?:i|1|l){4}|(?:e|3){4}|(?:o|0){4}|(?:s|5){4}|[\d|_]{7}|(?:^|[^g])r(?:a|4)p(?:e|3)|(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d|b(?:a|4)b(?:o|0){2,}n|g(?:o|0)r(e|3)|h(?:a|4)t(?:e|3)|pt(?:s|5)d|h(i|1|l)t(?:l|i|1)(?:e|3)r|(?:n|r|1|l)(?:i|1|l)(?:g|9){2,}(?:(?:e|3|o|0)r|uh|a|4)|n(?:e|3)(?:g|9)+(?:(?:e|3|o|0)r|uh|(?:a|4)(?:[^a-z]|$))|n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))|d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n|fr(?:i|1|l)(?:e|3)nd.*v(?:e|3)t(?:e|3)r(?:a|4)n|h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n|v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d|v(?:e|3)t(?:e|3)r(?:a|4)n.*fr(?:i|1|l)(?:e|3)nd|v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)|h(?:o|0)(?:s|5){2}|(?:0|o){2}3(?:1|i|l)|(?:0|o)3(?:1|i|l)[0-9]|(?:g|9)u(?:n|m)z(?:0|o)|(?:j|i){2}bu(?:i|1|l){2}d|(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)|(?:l|1|i)(?:a|4)r(?:s|5)h|(?:l|1|i)un(?:a|4)r|(?:o|0){2,}(?:l|i|1){2}(?:g|9)(?:a|4)n|(?:s|5)(?:i|1|l)m(?:o|0)+(?:l|i|1){2}|b(?:l|1|i)u(?:e|3)b(?:e|3)rr(?:y|i)d(?:o|0)g|k(?:i|1|l){3}.*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*k(?:i|1|l){3}|(?:g|9)(?:a|4)(?:s|5).*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*(?:g|9)(?:a|4)(?:s|5)|murd(?:e|3)r.*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*murd(?:e|3)r|dr(?:o|0)wn.*(?:j|i)(?:e|3)w|(?:j|i)(?:e|3)w.*dr(?:o|0)wn|(?:g|9)(?:a|4)(?:s|5).*ch(?:a|4)mb(?:e|3)r|k(?:i|1|l){3}.*(?:g|9)(?:a|4)(?:y|i)|(?:g|9)(?:a|4)(?:y|i).*k(?:i|1|l){3}|(?:g|9)(?:a|4)(?:s|5).*(?:g|9)(?:a|4)(?:y|i)|(?:g|9)(?:a|4)(?:y|i).*(?:g|9)(?:a|4)(?:s|5)|murd(?:e|3)r.*(?:g|9)(?:a|4)(?:y|i)|(?:g|9)(?:a|4)(?:y|i).*murd(?:e|3)r|dr(?:o|0)wn.*(?:g|9)(?:a|4)(?:y|i)w|(?:g|9)(?:a|4)(?:y|i).*dr(?:o|0)wn|^gu[a-z]+da$|^gun[a-z][0-9]+$``

## Individual filters
You do not need these if you use the one above.
Pick and choose from these filters if the one on top is too strict for you.

### Suspicious name structure
* **4+ consequent repeated letters**: ``regex:(.)\1{4}``
* **4+ consequent identical looking characters**: ``regex:(?:i|1|l){4}|(?:e|3){4}|(?:o|0){4}|(?:s|5){4}``
* **multiple underscores at end of name (against impersonation)**: ``regex:__$``
* **7+ consequent numbers (against phone number doxxing)**: ``regex:[\d|_]{7}``
* **gu...da**: ``regex:^gu[a-z]+da$``
* **gunxX**: ``regex:^gun[a-z][0-9]+$``

### Impersonated account names
* **0031**: ``regex:(?:0|o){2}3(?:1|i|l)``
* **031X**: ``regex:(?:0|o)3(?:1|i|l)[0-9]``
* **blueberrydog**: ``regex:b(?:l|1|i)u(?:e|3)b(?:e|3)rr(?:y|i)d(?:o|0)g``
* **gunz0**: ``regex:(?:g|9)u(?:n|m)z(?:0|o)``
* **hoss**: ``regex:h(?:o|0)(?:s|5){2}``
* **jjbuild**: ``regex:(?:j|i){2}bu(?:i|1|l){2}d``
* **judgejudy**: ``regex:(?:j|i)ud(?:g|9)(?:e|3)(?:j|i)ud(?:y|i)``
* **larsh**: ``regex:(?:l|1|i)(?:a|4)r(?:s|5)h``
* **lunar**: ``regex:(?:l|1|i)un(?:a|4)r``
* **ooligan**: ``regex:(?:o|0){2,}(?:l|i|1){2}(?:g|9)(?:a|4)n``
* **simooli**: ``regex:(?:s|5)(?:i|1|l)m(?:o|0)+(?:l|i|1){2}``

### Bad terms
* **baboon**: ``regex:b(?:a|4)b(?:o|0){2,}n``
* **gore**: ``regex:g(?:o|0)r(?:e|3)``
* **hate**: ``regex:h(?:a|4)t(?:e|3)``
* **hitler**: ``regex:h(i|1|l)t(?:l|i|1)(?:e|3)r``
* **ptsd**: ``regex:pt(?:s|5)d``
* **rape (but not grape)**: ``regex:(?:^|[^g])r(?:a|4)p(?:e|3)``
* **suicid**: ``regex:(?:s|5)u(?:i|1|l)(?:c|z)(?:i|1|l)d``

### Hate Speech against People of Color
* **nigger and variants (1/3)**: ``regex:(?:n|r|1|l)(?:i|1|l)(?:g|9){2,}(?:(?:e|3|o|0)r|uh|a|4)``
* **nigger and variants (2/3)**: ``regex:n(?:e|3)(?:g|9)+(?:(?:e|3|o|0)r|uh|(?:a|4)(?:[^a-z]|$))``
* **nigger and variants (3/3)**: ``regex:n(?:i|1|l|e|3)(?:g|9)+(?:(?:e|3)tt|r(?:e|3)(?:s|5)|r(?:a|4))``

### Hate Speech against LGBTQIA+
* **drown...gay**: ``regex:dr(?:o|0)wn.*(?:g|9)(?:a|4)(?:y|i)w``
* **gas...gay**: ``regex:(?:g|9)(?:a|4)(?:s|5).*(?:g|9)(?:a|4)(?:y|i)``
* **gay...drown**: ``regex:(?:g|9)(?:a|4)(?:y|i).*dr(?:o|0)wn``
* **gay...gas**: ``regex:(?:g|9)(?:a|4)(?:y|i).*(?:g|9)(?:a|4)(?:s|5)``
* **gay...kill**: ``regex:(?:g|9)(?:a|4)(?:y|i).*k(?:i|1|l){3}``
* **gay...murder**: ``regex:(?:g|9)(?:a|4)(?:y|i).*murd(?:e|3)r``
* **kill...gay**: ``regex:k(?:i|1|l){3}.*(?:g|9)(?:a|4)(?:y|i)``
* **murder...gay**: ``regex:murd(?:e|3)r.*(?:g|9)(?:a|4)(?:y|i)``

### Hate Speech against Religious Groups
* **drown...jew**: ``regex:dr(?:o|0)wn.*(?:j|i)(?:e|3)w``
* **gas...chamber**: ``regex:(?:g|9)(?:a|4)(?:s|5).*ch(?:a|4)mb(?:e|3)r``
* **gas...jew**: ``regex:(?:g|9)(?:a|4)(?:s|5).*(?:j|i)(?:e|3)w``
* **jew...drown**: ``regex:(?:j|i)(?:e|3)w.*dr(?:o|0)wn``
* **jew...gas**: ``regex:(?:j|i)(?:e|3)w.*(?:g|9)(?:a|4)(?:s|5)``
* **jew...kill**: ``regex:(?:j|i)(?:e|3)w.*k(?:i|1|l){3}``
* **jew...murder**: ``regex:(?:j|i)(?:e|3)w.*murd(?:e|3)r``
* **kill...jew**: ``regex:k(?:i|1|l){3}.*(?:j|i)(?:e|3)w``
* **murder...jew**: ``regex:murd(?:e|3)r.*(?:j|i)(?:e|3)w``

### Hate Speech against Veterans
* **dead...veteran**: ``regex:d(?:e|3)(?:a|4)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **died...veteran**: ``regex:d(?:i|1|l)(?:e|3)d.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **friend...veteran**: ``regex:fr(?:i|1|l)(?:e|3)nd.*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **haha...veteran**: ``regex:h(?:a|4)h(?:a|4).*v(?:e|3)t(?:e|3)r(?:a|4)n``
* **veteran...commit**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*c(?:o|0)mm(?:i|1)tt``
* **veteran...dead**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:e|3)(?:a|4)d``
* **veteran...died**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*d(?:i|1|l)(?:e|3)d``
* **veteran...friend**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*fr(?:i|1|l)(?:e|3)nd``
* **veteran...haha**: ``regex:v(?:e|3)t(?:e|3)r(?:a|4)n.*h(?:a|4)h(?:a|4)``
