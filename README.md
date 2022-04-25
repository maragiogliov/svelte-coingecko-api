
---

# svelte app

Searching functionality problem:    

'cardano' === 'Cardano'   false
'card' === 'Cardano'   false

Solution:

'Cardano'.toLowerCase().include('card')  true
'Cardano'.toLowerCase().include('ard')  true
'Cardano'.toLowerCase().include('rd')  true

in Code:

const searchCoin = (value)=>{
	coins = coins.filter((coin)=> 
	coin.name.toLowerCase().includes(value.toLowerCase())
	)
}

We filter the coinList depending of the user input, we compare input value with coin.name
update the value of {coins} 
See if there is any value included and we counted as 'Cardano', 
also  to lowerCase both (INPUT and API value coin.name) for accurate comparison




```
