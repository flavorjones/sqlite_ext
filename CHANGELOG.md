### 0.3.0 - 2016-06-23
* Removals
  * Removed support for a block argument to `SqliteExt.register_function`.
    It now accepts a `Proc` passed as a standard argument instead.
* Enhancements
  * Functions registered using `SqliteExt.register_function` automatically
    propagate `NULL` when `NULL` is passed for one or more of the required
    parameters of the `Proc` that performs the function.
