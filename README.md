# Colony

[![Tests](https://github.com/LlewVallis/colony/actions/workflows/ci.yml/badge.svg)](https://github.com/LlewVallis/colony/actions/workflows/ci.yml)
[![Crates.io](https://img.shields.io/crates/v/colony)](https://crates.io/crates/colony)
[![Docs](https://img.shields.io/docsrs/colony)](`https://docs.rs/colony`)

An unordered data-structure with `O(1)` lookup, removal, iteration and `O(1)` amortized insertion.
Like a faster `HashMap` that chooses its own keys.
Also similar to a `Vec<Option<T>>`, where instead of calling `Vec::remove` elements are removed by setting the element to `None`.

See [the documentation](https://docs.rs/colony) for more information.

This crate is partly a port of [`plf::colony`](https://plflib.org/colony.htm), which is a
[proposed addition](https://isocpp.org/files/papers/P0447R16.html)
to the C++ standard library under the name `std::hive`.