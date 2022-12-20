# C
## Getting started
## Control statements
### Conditional execution
 - `if` construct
  ```c
  if (condition)
    statement0-or-block0
  else
    statement1-or-block1
  ```
 - Conditons: the value 0 represents logical false while non-zero is logical true. The 'bool' type exists but requires standard library
 - Rule of thumb: NEVER compare to 0, 'false', or 'true'
### Iterations
 - `for` construct
  ```c
  for (clause1; condition2; expression3)
    statement-or-block
  ```
 - `while` construct
  ```c
  while (condition)
    statement-or-block
  ```
 - `do` construct (`statement-or-block` is executed at least once)
  ```c
  do
    statement-or-block
  while (condition);
  ```
 - C convention of `while(true)`
  ```c
    for (;;)
      statement-or-block
  ```
### `switch`
  - An example
  ```c
      switch (arg) {
        case 'm':
          puts("this is a magie");
          break;
        case 'r':
          puts("this is a raven");
          break;
        case 'j':
          puts("this is a jay");
          break;
        default:
          puts("this is an unknown corvid");
  }
  ```
 - Fall through behavior: `break` is necessary otherwise all statements after hit case will be executed. For example, `arg='m'` will print all statements including default case
 - `case` must be integer constant expressions.
