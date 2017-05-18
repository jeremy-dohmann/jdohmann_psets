Generation rules:
=================


Begin with F1 rules:
--------------------


Attempt to lexify each unlexified item.
Look appropriate lexifications by finding appropriate semification 
then extracting value from frame.

E.G.

Resolve F1.Agent rules to F1.Experiencer wish is "I", lexify F1.Object to F1.Event.

Lexify F2.Agent to F2.Buyer which is "Bill". Lexify F2.Object to F2.Goods which is "a car."

Final produce the final output which is "I" + "wish (that)" + "Bill" + "bought" + "a car."

Frames
------

| F1 = Desire       | F2 = Commerce_buy |
|-------------------|-------------------|
| vb = wish         | vb = bought       |
| Experiencer = "I" | Buyer = "Bill"    |
| Event = F2        | Goods = "a car"   |


Rules
-----

| F1                    | F2                  |
|-----------------------| --------------------|
| Agent wish (that) Obj | Agent bought Object |
| Experiencer $ Agent   | Buyer $ Agent       |
| Event $ Object        | Goods $ Object      |

