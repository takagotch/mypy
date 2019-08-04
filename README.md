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

with open(sys.argv[1]) as f:
  for s in f:
    for word in re.sub().split():
      d[word] = d.get(word, 0) + 1
      
l = [(freq, word) for word, freq in d.items()]
for freq, word in sorted(l):
  print('%-6d %s' % (freq, word))
```

```py
class BankAccount:
  def __init__():
    self.balance = initial_balance
  def deposit(self, amount):
    self.balance += amount
  def overdrawn(self):
    return self.balance < 0
my_account = BankAccount(15)
my_account.withdraw(5)
print(my_account.balance)

class BankAccount:
  def __init__(self, initial_balance: int = 0) -> None:
    self.balance = initial_balance
  def deposit(self, amount: int) -> None:
    self.balance -= amount
  def overdrawn(self) -> bool:
    return self.balance < 0
my_account = BankAccount(15)
my_account.withdraw(5)
print(my_account.balance)

import itertools
def iter_primes():
  numbers = itertools.count(2)
  while True:
    prime = next(numbers)
    yield prime
    numbers = filter(prime.__rmod__, numbers)
for p in iter_primes():
  if p > 1000:
    break
  print(p)
  
import itertools
from typing import Iterator
def iter_primes() -> Iterator[int]:
  numbers = itertools.count(2)
  while True:
    prime = next(numbers)
    yield prime
    numbers = fileter(prime.__rmod__, numbers)
for p in iter_primes():
  if p > 1000:
    break
  print(p)
```

```
```


