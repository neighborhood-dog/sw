Instructions from <https://github.com/peyo-hd/vendor_nvdla/commit/c09818346e7f8010ef632f82529708dc030e4eb8>,
modified to compile using riscv64. Corrected paths to copy libprotobuf.a to.

 enable host compiler build

  How to build protobuf library
   $ cd umd/external/protobuf-2.6
   $ ./configure --build=riscv64-unknown-linux-gnu
   $ TOP=$(pwd) make -jxx
  copy libprotobuf.a to umd/core/src/compiler & umd/apps/compiler folder

  How to build nvdla_compiler
   $ cd umd
   $ TOP=$(pwd) make -jxx
  check umd/out/ folder
