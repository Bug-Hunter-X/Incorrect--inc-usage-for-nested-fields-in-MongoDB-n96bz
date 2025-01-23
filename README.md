# Incorrect $inc Usage for Nested Fields in MongoDB
This example demonstrates an uncommon error in MongoDB when using the `$inc` operator to update nested fields. The problem occurs when the dot notation for accessing nested fields is not used correctly within the `$inc` operator.  The solution shows how to use dot notation properly to correctly increment the nested field.

## Bug
The `$inc` operator fails to update a nested field if the field path isn't properly specified using dot notation.  This results in either no change or unexpected behavior depending on the specifics of the update operation. 

## Solution
The correct approach involves using dot notation (`nested.field`) to accurately target the nested field within the `$inc` operator. This ensures the value is incremented as expected. 