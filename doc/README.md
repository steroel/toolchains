# README

from [Bliazard: Bazel - C/C++ toolchain from scratch](https://www.youtube.com/watch?v=5ugdNGVjSRQ&list=PLHyFZPM7nk3SV4y_1FxCCMdJLhKWLFjgS&index=10)

```powershell
bazel fetch @arm_gcc//...

tree -L 2 $(bazel info output_base)/external

bazel run example --platforms=//toolchain_arm_gcc:platform -s

bazel run example --incompatible_enable_cc_toolchain_resolution --platforms=//toolchain_arm_gcc:platform -s

```
