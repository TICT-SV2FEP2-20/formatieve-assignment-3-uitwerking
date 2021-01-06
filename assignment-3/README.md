# Assignment 3

De applicatie gaat z'n state door middel van Redux bij houden.

De state moet gaan bestaan uit twee slices. Een Cart en een Products slice.

## Cart:

De cart exposed de volgende actions: 

* `add` - Accepteert een action met als payload: `{ category, id }`
* `remove` - Accepteert een action met als payload: `{ id }`
* `setQuantity` - Accepteert een action met als payload: `{ id, quantity }`
 
Vervolgens exposed de cart de volgende derived state:

* `getProducts`
* `getTotalPrice`
* `isProductInCart`

## Products

De products slice exposed de volgende actions:

* `saveProducts` - Accepteert een action waarvan de volledige payload als nieuwe
                   state geldt
* `removeProduct` - Accepteert een action met als payload `{ id }`

vervolgens exposed de cart de volgende derived state:

* `getProducts`
* `getProduct`
* `getCategory`