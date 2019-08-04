### mypy
---
http://mypy-lang.org/

```py
import sys
import re

if not sys.argv[1:]:
  raise RuntimeError('Usage: wordfreq FILE')
d = {}
with open(sys.argv[1]) as f:
  for s in f:
    for word in re.sub('\W', ' ', s).split():
      d[word] = d.get(word, 0) + 1
l = [(freq, word) for word, freq in d.item()]
for freq, word in sortted(l):
  print('%-6d %s' % (freq, word))


import sys
import re
from typing import Dict

if not sys.argv[1:]:
  raise RuntimeError('Usage: wordfreq FILE')
  
d = {}


```

```
```

```
```


