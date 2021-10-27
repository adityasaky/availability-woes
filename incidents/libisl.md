# Integer Set Library (libisl)

This was a relatively low profile situation as it didn't outright cause breakages because of how dependent packages handled the dependency. ISL is "a library for manipulating sets and relations of integer points bounded by linear constraints", according to their official website. It was reported in October 2021 that the official site maintained by the developers of the library was down, and had been for several days, making it impossible for developers to fetch its latest versions. High profile dependents of this package include both GCC and LLVM.

To add to the unavailability concern, the library was distributed from a privately managed host via HTTP only, and this could have been the target for a supply chain attack in multiple ways. The developers have since also begun distributing the package via SourceForge.

The reason neither GCC nor LLVM broke because of the unavailability of the package was that both projects stored a copy of the library themselves. GCC stored a copy of the archive which it fetched via a pre-requisite script run during the build, while LLVM vendored the code into its source tree.

## Sources

1. Official Website: https://libisl.sourceforge.io/, archived at https://archive.is/mwQmt
2. Mailing List thread detailing infrastructure being down: https://groups.google.com/g/isl-development/c/JGaMo2VUu_8, archived at https://archive.is/Qk7yN
3. GCC copy of library: https://gcc.gnu.org/pub/gcc/infrastructure/, archived at https://archive.is/oAoUL
4. GCC script to fetch library: https://gcc.gnu.org/git/?p=gcc.git;a=blob;f=contrib/download_prerequisites;h=11c283ecb1aab88958915cff65109ddd5801a9e1;hb=HEAD#l33, archived at https://archive.md/aTiHS
5. LLVM vendored copy of library source: https://github.com/llvm/llvm-project/tree/722a2fb7f9a3f7deea81276213c6a2a48a0827cd/polly/lib/External/isl, archived at https://archive.md/EZ0em
