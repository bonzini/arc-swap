* Both `swap` and `load` (and similar methods) are now lock-free (but not
  wait-free). Currently, a backend very similar to hazard pointers is used.
* Signal safety needs to be explicitly requested (as there's worse performance
  and only limited lock-freeness in that case).

# 0.1.4

* The `peek` method to use the `Arc` inside without incrementing the reference
  count.
* Some more (and hopefully better) benchmarks.

# 0.1.3

* Documentation fix (swap is *not* lock-free in current implementation).

# 0.1.2

* More freedom in the `rcu` and `rcu_unwrap` return types.

# 0.1.1

* `rcu` support.
* `compare_and_swap` support.
* Added some primitive benchmarks.

# 0.1.0

* Initial implementation.
