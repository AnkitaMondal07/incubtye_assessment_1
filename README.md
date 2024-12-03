# incubtye_assessment_1
Features
Returns 0 for an empty string.
Adds numbers separated by commas (,) or newlines (\n).
Supports:
Custom single-character delimiters.
Custom delimiters of any length.
Multiple custom delimiters of varying lengths.
Ignores numbers greater than 1000.
Throws exceptions for negative numbers, listing all negatives in the error message.



Empty String:
expect(add("")).toBe(0);

Single Number:
expect(add("1")).toBe(1);

Custom Delimiter:
expect(add("//;\n1;2")).toBe(3);

Multiple Delimiters
expect(add("//[*][%]\n1*2%3")).toBe(6);

Negative Numbers:
expect(() => add("1,-2,3")).toThrow("negative numbers not allowed: -2");


# To run all test cases
npm test