## Summary

Constants: `let`
Variables: `var`

built-in arithmetic operators, such as `+`, `-`, `*`, and `/` can be shortend to `+=`, `-=`, `*=`, and `/=` if just variable itself should be changes. 
Example: `counter = counter + 1` => `counter += 1`



String holds text:
String interpolation works with `\(var/let)` but can only be a var if the string is also a var. 
`let playerName: String = "Roy"`

Int holds whole numbers:
`var luckyNumber: Int = 13`

Double holds decimal numbers:
`let pi: Double = 3.141`

Bool holds either true or false:
Booleans can be flipped with `.toogle()`
`var isAuthenticated: Bool = true`

Array holds lots of different values, all in the order they are added using integer indices. `[datatyp]`
helpful functionality: 
* count
* append() 
* contains()
`var albums: [String] = ["Red", "Fearless"]`

Dictionary holds lots of different values, where the key decides how data should be accessed, similar functionality to arrays. `[Datatyp of Key: Datatyp of Value]`
`var user: [String: String] = ["id": "@twostraws"]`

Set holds lots of different values, but stores them in an order that’s optimized for checking what it contains. And can contain any value only once. `Set<datatyp>`
`var books: Set<String> = Set(["The Bluest Eye", "Foundation", "Girl, Woman, Other"])`

Type annotations are not needed:
`var soda: [String] = ["Coke", "Pepsi", "Irn-Bru"]`
Only for empty array, dict or set.
`var teams: [String] = [String]()`

Values of an enum have the same type as the enum itself. Can specify a range of acceptable values such as a list of actions the user can perform, the types of files we are able to write, or the types of notification to send to the user
```
enum UIStyle {
    case light, dark, system
}
var style = UIStyle.light
```

type annotations for empty constants
```
let username: String
username = "@twostraws"
print(username)
```

Swift must always know the type of data inside a constant or variable, and mostly uses type inference to figure that out based on the data we assign. However, it’s also possible to use type annotation to force a particular type.


`if` statements to check a condition 
`else` block, and/or multiple `else if` blocks to check other conditions

`||` or 
`&&` and 

`switch` if same kinds of check is repeated alot
`fallthrough` executes the following case aswell

`for` loop over arrays, sets, dictionaries, and ranges. assign items to a loop variable and use it inside the loop. to ignore the loop variable underscore `_`can be used.
`while` craft custom loops that will continue running until a condition becomes false.
`continue` skip the rest of the loop and starts at the next itteration. 
`break` ends the loop
