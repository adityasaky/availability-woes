# Cargo

Cargo is Rust's official package manager, and packages (or crates) are fetched from the online index, crates.io.

## Yanking or Deletion of Versions

In the world of crates.io, "yanking" has a slightly different definition from some of the other package indexes. Yanking a version of a crate does not delete the underlying code, but rather ensures no new dependencies can be formed on that particular version. On the other hand, existing dependencies on that version will continue to work as before.

## Deletion of Projects / Potential for Squatting

crates.io doesn't allow developers to directly unpublish or delete a published crate. At best, they can yank the crate, and contact the registry to discuss deletion options. However, as of 2018, the maintainers of the repository indicated that they don't remove crates for any reason other than legal requests or code of conduct violations.

This policy means that it is harder, or indeed impossible, for the namespace of a crate to be occupied by a different developer post some deletion activity. However, the community has previously pointed out that many significant names have already been preemptively squatted by users. This can possibly lead to typosquat or dependency confusion situations.

## Sources

1. cargo yank: https://doc.rust-lang.org/cargo/reference/publishing.html#cargo-yank, archived at https://archive.md/I2brC
2. Discussion on GitHub indicating that crate removal requests are rarely entertained: https://github.com/rust-lang/crates.io/pull/1506, archived at https://archive.md/MaatH
3. Could Rust have a left-pad incident?: https://edunham.net/2016/03/24/could_rust_have_a_left_pad_incident.html, archived at https://archive.md/fX8VP
4. GitHub thread which includes input from crates.io admin: https://github.com/servo/servo/issues/10142, archived at https://archive.md/Dv9jN