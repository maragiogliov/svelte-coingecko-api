
---

# svelte app

Searching functionality problem:

'cardano' === 'Cardano'   false
'card' === 'Cardano'   false

Solution:

'Cardano'.toLowerCase().include('card')  true
'Cardano'.toLowerCase().include('ard')  true
'Cardano'.toLowerCase().include('rd')  true





```
