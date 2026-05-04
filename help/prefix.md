{.compact}
Label   | Type  | Description
---     | ---   | ---
Flag    | bool  | A boolean variable that can be either true or false.
Int     | int   | An integer variable used to store whole numbers.
String  | string| A variable used to store a sequence of characters.

{.compact}
Prefix | Label        | Description
---    | ---          | ---
F      | Fast         | A regular fastvariable that is initialized once and does not change until a new session begins.
DF     | Dynamic Fast | A fastvariable that can change at run-time, and automatically updates every 5 minutes.
