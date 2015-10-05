1. Assign the value `6` to the variable `number_six`

number_six = 6

2. What is the datatype of `"Matz"`?

String

3. What do the following expressions evaluate to:
  * `"Cool" + "Cool" + "Cool"`

"CoolCoolCool"

  * `t = "Troy"
    a = "Abed"
    "#{t} and #{a} in the Morning"`

"Troy and Abed in the Morning"

  * `10 * 3`

30

  * `10 ** 3`

1000

  * `10 % 3`

1

  * `10 / 3`

3

  * `0.7 + 0.1`

0.7999999999999999

4. Can you explain why the expressions all give the same result?
  * `"Ronnie " + "Pickering"`
  * `"Ronnie ".+("Pickering")`
  * `"Ronnie ".send(:+, "Pickering")`

+ is a string method, so thanks to Ruby syntactical sugar we can write it as:

"Ronnie " + "Pickering"

but it can also be used with the normal method syntax as in the second example:

"Ronnie ".+("Pickering")

In the third example, the send method is passed the + method as a symbol, and a string as the second argument. Send invokes whatever method it is passed, and passes it the specified arguement (in this case "Pickering"). So this is effectively the same as the other two approaches above. 


5. Please fix the following buggy expressions:
  * `number six = 6`
  * `"Maroon" + 5`
  * `ture == flase`

  number_six = 6
  "Maroon" + " 5"
  true == false
