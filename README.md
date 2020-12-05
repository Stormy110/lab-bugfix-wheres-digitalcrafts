# Where's DigitalCrafts?

This program displays the states which have cities named "Atlanta", "Houston", "Tampa".

# Bugs to fix

- [X] After lots of debugging, code stopped running. `node index.js` does nothing
-         **** Uncommented the main() function call ***
- [X] Started crashing after adding "tampa" search
-         **** Added db. in front of statesWithCity in the Tampa function ****
- [X] Prints "Atlanta" locations twice (instead of Houston)
_         **** Changed the statesWithHouston function callback for loop to include ****
          **** statesWithAHouston instead of statesWithAnAtlanta ****

For each bug you fix, add documentation to this README about how you fixed it (include before/after code samples).

# For the more curious:

`db.js` includes more functions that you can try out. In `index.js`, try to `console.log()` the results of the following function calls:

- `getByAbbreviation('ak')`
- `searchByName('dakota')`
  - Why does this only return results for North Dakota (and not South Dakota)?
  _     **** In the findIndex function call, it only returns the first element in the ****
        **** array that returns true. Since North comes before South alphabetically and ****
        **** (more importantly) in the array, north dakota is returned ****
