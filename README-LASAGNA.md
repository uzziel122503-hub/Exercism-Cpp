Notes while debugging
Treating function name as a variable
  What I wrote: remainingOvenTime = ...
  What I should have written: return ...
  Why it failed: Function names aren't variables; you can't assign values to them. Use return to output the result.
Missing function call parentheses
  What I wrote: ovenTime
  What I should have written: ovenTime()
  Why it failed: Without (), the compiler sees the function address, not the result of calling it.
Missing return statement
  What I wrote: No return keyword
  What I should have written: return ovenTime() - actualMinutesInOven;
  Why it failed: Function declares int return type but didn't return anything. Compiler error/warning.
Key Takeaways for Portfolio Notes
  Functions are called with () — always include parentheses even if there are no arguments
  Return types must be honored — if you declare int, you must return an integer
  Don't assign to function names — use return to send values back to the caller
  DRY Principle — Don't Repeat Yourself. Call ovenTime() instead of hardcoding 40 so changes only need to happen in one place
