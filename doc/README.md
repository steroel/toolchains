# README

```powershell
bazel fetch @arm_gcc//...

tree -L 2 $(bazel info output_base)/external

bazel run example --platforms=//toolchain_arm_gcc:platform -s

bazel run example --incompatible_enable_cc_toolchain_resoution --platforms=//toolchain_arm_gcc:platform -s

```
