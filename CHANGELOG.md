# Changelog

## [0.3.0](https://github.com/teepean/bwa-mem3/compare/v0.2.1...v0.3.0) (2026-05-20)


### Features

* --bam[=LEVEL] output flag for direct BAM emission ([#12](https://github.com/teepean/bwa-mem3/issues/12)) ([84defc3](https://github.com/teepean/bwa-mem3/commit/84defc3bb6b3405f7a23ea9265dc582258032d02))
* add CI workflow with cross-platform build and end-to-end test ([744a9e7](https://github.com/teepean/bwa-mem3/commit/744a9e77d5cbde91b804b720d6e03cf11f75de5a))
* **arm64:** make Linux aarch64 build + CI-test on every fg-main push ([#1](https://github.com/teepean/bwa-mem3/issues/1)) ([5132582](https://github.com/teepean/bwa-mem3/commit/5132582fa96969eb8b9304c9e5d515691d17c284))
* **bns:** convert mem_matesw_batch_{pre,post} to bns_fetch_seq_v2 ([#76](https://github.com/teepean/bwa-mem3/issues/76)) ([af33cdd](https://github.com/teepean/bwa-mem3/commit/af33cdd834747d7d9a890228b8e09cd94d121cf7))
* **cli:** wire up --help across commands; add -h to top-level and index ([#60](https://github.com/teepean/bwa-mem3/issues/60)) ([d8d4a6d](https://github.com/teepean/bwa-mem3/commit/d8d4a6d25f5b6cbd0f63cea59ece01501e970017))
* expose worker_alloc/worker_free, the core worker_t pre-allocation helpers ([#8](https://github.com/teepean/bwa-mem3/issues/8)) ([6b76c7b](https://github.com/teepean/bwa-mem3/commit/6b76c7b6a6f4d3f05832dbcb49cbd9a76d85f94b))
* **hdr:** export mem_infer_dir for external consumers ([#6](https://github.com/teepean/bwa-mem3/issues/6)) ([b27f374](https://github.com/teepean/bwa-mem3/commit/b27f3743769bac4a165129eeaa28893037243eb5))
* **index:** libsais-based memory-bounded FM-index construction ([#57](https://github.com/teepean/bwa-mem3/issues/57)) ([79b90ce](https://github.com/teepean/bwa-mem3/commit/79b90ce7ae6da29da96bf573c6634b1155c2979a))
* **makefile:** parameterize PGO targets by arch + profile dir ([#59](https://github.com/teepean/bwa-mem3/issues/59)) ([57e21bd](https://github.com/teepean/bwa-mem3/commit/57e21bd9e15b1a28e9f5bb9f740e754a0e2c8f40))
* **mapq:** add --supp-rep-hard-cap opt-in supp MAPQ rescoring ([#56](https://github.com/teepean/bwa-mem3/issues/56)) ([595d8e5](https://github.com/teepean/bwa-mem3/commit/595d8e5988598cd994d5beb1e58a01438809920d))
* **mem:** emit HN:i tag with total hit count per primary ([#42](https://github.com/teepean/bwa-mem3/issues/42)) ([93a79ec](https://github.com/teepean/bwa-mem3/commit/93a79ec171e2e5ae56cb7d38e6c5802eadfe1eb0))
* **meth:** --meth + `index --meth` — bwameth.py-equivalent bisulfite mode ([#13](https://github.com/teepean/bwa-mem3/issues/13)) ([7641ebf](https://github.com/teepean/bwa-mem3/commit/7641ebf1d9aa1da94da5886610a0d33e8e2ad5b6))
* **meth:** emit Bismark-compatible XR/XG/XM auxiliary tags ([#90](https://github.com/teepean/bwa-mem3/issues/90)) ([ec67b09](https://github.com/teepean/bwa-mem3/commit/ec67b0908997aeb754f7b589c0c39f060ae74bb9))
* rename meth PG header to bwa-mem3-meth and drive VN from PACKAGE_VERSION ([7a56f9a](https://github.com/teepean/bwa-mem3/commit/7a56f9a25b96f0d27735cc5d18883c44d4127868))
* rename PG header to bwa-mem3 (ID, PN, usage strings) ([bb919f2](https://github.com/teepean/bwa-mem3/commit/bb919f290c533727f6f18feaa33afc0609a60e6c))
* **shm:** add `bwa-mem2 shm --meth` for symmetric meth UX ([#67](https://github.com/teepean/bwa-mem3/issues/67)) ([c20f61c](https://github.com/teepean/bwa-mem3/commit/c20f61cad961f90c3f7932e524335c70c5555273))
* **shm:** port `bwa shm` from bwa-mem v1 ([#65](https://github.com/teepean/bwa-mem3/issues/65)) ([20f77e9](https://github.com/teepean/bwa-mem3/commit/20f77e9fe9fb1910045ded014afaa8c0f1e684a7))
* **shm:** serialize /bwactl RMW with a POSIX named semaphore ([#82](https://github.com/teepean/bwa-mem3/issues/82)) ([ddfb0da](https://github.com/teepean/bwa-mem3/commit/ddfb0da97d3711c6a761116a447f80ea05b80ac3))
* **simd:** add SIMD host-floor precheck for multi-arch deployment ([#95](https://github.com/teepean/bwa-mem3/issues/95)) ([dc7fcfe](https://github.com/teepean/bwa-mem3/commit/dc7fcfe57ee95f216c1be107d82a0e827fa3bfa3))
* **simd:** replace multi-binary execv launcher with single-binary in-process dispatch ([#83](https://github.com/teepean/bwa-mem3/issues/83)) ([b9e0b66](https://github.com/teepean/bwa-mem3/commit/b9e0b66b908544a06c36bac336ad7eaa1e749926))
* split mem_sam_pe into mem_pair_resolve + thin emission wrapper ([#9](https://github.com/teepean/bwa-mem3/issues/9)) ([e80765b](https://github.com/teepean/bwa-mem3/commit/e80765bbedeeebf137608ba3e23db0672d6aa937))
* vendor mimalloc v3.3.0 and link by default ([#19](https://github.com/teepean/bwa-mem3/issues/19)) ([73907d7](https://github.com/teepean/bwa-mem3/commit/73907d7517ab92509fc4599baf2df51df7e468fd))


### Bug Fixes

* **bntseq:** bound .alt parse buffer to prevent stack overflow ([#74](https://github.com/teepean/bwa-mem3/issues/74)) ([b3a665e](https://github.com/teepean/bwa-mem3/commit/b3a665ee713f214ea810e33567f3c6c4a034ccec))
* **changelog:** strip preamble so release-please owns the file ([#112](https://github.com/teepean/bwa-mem3/issues/112)) ([56e580c](https://github.com/teepean/bwa-mem3/commit/56e580cf4f2515280440b2882a32c3a6a7b6d15c))
* compute no_pairing 0x2 flag from the emitted alignment ([#17](https://github.com/teepean/bwa-mem3/issues/17)) ([8944028](https://github.com/teepean/bwa-mem3/commit/894402828beb261d3bee5caec06e6b9e33d8e916))
* drop unused global `stat` that shadows libc ([490502b](https://github.com/teepean/bwa-mem3/commit/490502b238d0da3799c436caf2da5bb6081fd178))
* **fmi:** parenthesize SA_COMPX_MASK precedence in sampled-SA prefetch ([#73](https://github.com/teepean/bwa-mem3/issues/73)) ([442de25](https://github.com/teepean/bwa-mem3/commit/442de25a1ddf9ef1b196e52bc5771963d99307ab))
* **hdr:** align bwamem.h declarations with bwamem.cpp definitions ([#5](https://github.com/teepean/bwa-mem3/issues/5)) ([246b528](https://github.com/teepean/bwa-mem3/commit/246b5281d0dc6a2f6c45def30045df15a90c5627))
* **kswv:** apply NEON score2-scan fixes to AVX-512BW kernel ([#21](https://github.com/teepean/bwa-mem3/issues/21)) ([2fd0e96](https://github.com/teepean/bwa-mem3/commit/2fd0e96ac2e242b42d4cb10fe9a6cb0c5da3885e))
* **kswv:** apply score2 plateau fix + missing filters to kswv_512_16 ([#30](https://github.com/teepean/bwa-mem3/issues/30)) ([75c709a](https://github.com/teepean/bwa-mem3/commit/75c709a16d60a10db0b77ba14990a076a39c76ac))
* **kswv:** consolidate score2 plateaus per-lane to match scalar ksw_align2 ([#28](https://github.com/teepean/bwa-mem3/issues/28)) ([43457e8](https://github.com/teepean/bwa-mem3/commit/43457e80004d29bcd51c3f5569639bbdf271baac))
* **kswv:** gate AVX2 arch dispatch on !__AVX512BW__ ([#26](https://github.com/teepean/bwa-mem3/issues/26)) ([0bb9402](https://github.com/teepean/bwa-mem3/commit/0bb94028f0c601c4fb32d94bfa05bf5eea06a0e1)), closes [#25](https://github.com/teepean/bwa-mem3/issues/25)
* **kswv:** port score2 plateau consolidation to NEON + AVX-512BW ([#29](https://github.com/teepean/bwa-mem3/issues/29)) ([2311f11](https://github.com/teepean/bwa-mem3/commit/2311f1127d47393c5bcda07e40bda799f403a7f4))
* **kswv:** rewrite kswv_neon_16 — real SIMD kernel with correct table + score2 ([#31](https://github.com/teepean/bwa-mem3/issues/31)) ([61813ef](https://github.com/teepean/bwa-mem3/commit/61813ef66141196b5af5b1a0910c895820c91d5e))
* **mapq:** propagate SMEM SA-count to seed n_hits so --supp-rep-hard-cap works ([#101](https://github.com/teepean/bwa-mem3/issues/101)) ([cca9d4f](https://github.com/teepean/bwa-mem3/commit/cca9d4f41023e501636d2b1ebd2d1e825f95e8e3))
* **matesw:** copy ref slice before ksw_align2 to avoid SIGSEGV on shm-backed ref_string ([#85](https://github.com/teepean/bwa-mem3/issues/85)) ([316dba6](https://github.com/teepean/bwa-mem3/commit/316dba6240c9d9b41bcac6e965c77b41d9070af1))
* **profiling:** clamp display_stats nthreads to LIM_C ([#81](https://github.com/teepean/bwa-mem3/issues/81)) ([e65ceb2](https://github.com/teepean/bwa-mem3/commit/e65ceb27bde564c924a2a5430322a0e5564d4a62))
* **sam:** sanitize whitespace in -R when embedding into @PG CL: field ([#54](https://github.com/teepean/bwa-mem3/issues/54)) ([9b702ca](https://github.com/teepean/bwa-mem3/commit/9b702ca789ee24992d00863e87023ae7989060f9))
* **smem:** size SMEM buffers from observed max read length (closes [#44](https://github.com/teepean/bwa-mem3/issues/44)) ([#55](https://github.com/teepean/bwa-mem3/issues/55)) ([e22dade](https://github.com/teepean/bwa-mem3/commit/e22dade876ef7325c5299663404fd69bbda7221f))
* **smem:** track enc_qdb byte capacity separately from wsize_mem ([#100](https://github.com/teepean/bwa-mem3/issues/100)) ([ab922b6](https://github.com/teepean/bwa-mem3/commit/ab922b6af531ed4521b6cd9bd3c43a661d51a421))
* **test/meth:** alias bwa-mem2 -&gt; bwa-mem3 on PATH for bwameth.py oracle ([#72](https://github.com/teepean/bwa-mem3/issues/72)) ([2ea69db](https://github.com/teepean/bwa-mem3/commit/2ea69dbc521e4ecf60af8ff7f9e82a051b5f6f1d))
* zero bseq1_t in kseq2bseq1 so realloc'd entries don't carry garbage ([#22](https://github.com/teepean/bwa-mem3/issues/22)) ([0165b6c](https://github.com/teepean/bwa-mem3/commit/0165b6c2a39f784f16a4c3e4ce9e99188bb16eed))


### Performance

* **build:** default x86 single-binary baseline to avx2 (was sse41) ([#84](https://github.com/teepean/bwa-mem3/issues/84)) ([7d27f23](https://github.com/teepean/bwa-mem3/commit/7d27f231e1713a104385925ed3a90817f65645df))
* consolidated mapping speedups (ksw2, SMEM, SAL, SAM) ([#58](https://github.com/teepean/bwa-mem3/issues/58)) ([7301762](https://github.com/teepean/bwa-mem3/commit/7301762b08de2e15e0e61adf04ae498036a28510))
* **fmi:** bump SMEM_LOCKSTEP_N from 8 to 16 ([#75](https://github.com/teepean/bwa-mem3/issues/75)) ([000c0fd](https://github.com/teepean/bwa-mem3/commit/000c0fd523ca78f2daffd52c7cfc1dc120a332f3))
* **fmi:** inline backwardExt to recover gcc 12+ wall-clock regression ([#88](https://github.com/teepean/bwa-mem3/issues/88)) ([427c81c](https://github.com/teepean/bwa-mem3/commit/427c81cc4f1f2d095106e35a4bbe5a5efa386f0b))
* **header:** batch -H ingestion to fix O(n^2) header read (closes [#37](https://github.com/teepean/bwa-mem3/issues/37)) ([#49](https://github.com/teepean/bwa-mem3/issues/49)) ([ed63fad](https://github.com/teepean/bwa-mem3/commit/ed63fad0eaa994d28f8ce60924fa7346873dbaab))
* **ksort:** replace per-call malloc with on-stack buffer for small n ([#78](https://github.com/teepean/bwa-mem3/issues/78)) ([ff95a4f](https://github.com/teepean/bwa-mem3/commit/ff95a4f801fb1254283aac165313ce15d9fa47ca))
* **kswv:** add per-strip L1 prefetches to all u8/16 kernels ([#70](https://github.com/teepean/bwa-mem3/issues/70)) ([8137740](https://github.com/teepean/bwa-mem3/commit/8137740b1974e06d5758687561c484112069ffd5))
* **libsais_build:** skip wasted zero-init on unpack + SA buffers ([#80](https://github.com/teepean/bwa-mem3/issues/80)) ([fdb244d](https://github.com/teepean/bwa-mem3/commit/fdb244d3895eafa651a1a751c0ecfee1bf2f98ae))
* **seed:** lockstep SMEM batching across N reads ([#33](https://github.com/teepean/bwa-mem3/issues/33)) ([1f76655](https://github.com/teepean/bwa-mem3/commit/1f76655ecc183babdb3f704376cedc246f4a8625))
* **ungapped:** closed-form HIT for total_mis == 0 ([#77](https://github.com/teepean/bwa-mem3/issues/77)) ([7caf77c](https://github.com/teepean/bwa-mem3/commit/7caf77c083d04b09454cea234bbe03111523d8fb))
* **x86:** cap avx512bw autovec at 256-bit; bwa_shm /dev/shm preflight ([#86](https://github.com/teepean/bwa-mem3/issues/86)) ([c96d31a](https://github.com/teepean/bwa-mem3/commit/c96d31a0c8162db55a13ecfc0e540fc099c956c2))


### Refactoring

* rename bwa_mem2idx to bwa_mem3idx ([ee18a3b](https://github.com/teepean/bwa-mem3/commit/ee18a3b28e44c6295e49f0e61d321d050df913fa))


### Documentation

* add 0.1.0-pre release notes and update status.md ([924a70f](https://github.com/teepean/bwa-mem3/commit/924a70f602d86a47c0cfaf0b584ca276cbbb7ee2))
* add comprehensive mdbook on Read the Docs ([#71](https://github.com/teepean/bwa-mem3/issues/71)) ([41e1f3c](https://github.com/teepean/bwa-mem3/commit/41e1f3c43ca87de0cd60ee8d94331c42bb827b42))
* add FG-MAIN.md documenting the fork's relationship to upstream ([#3](https://github.com/teepean/bwa-mem3/issues/3)) ([db5086a](https://github.com/teepean/bwa-mem3/commit/db5086aef870adf30c9317069e1b7b1cdcf53281))
* drop README-ori.md (lineage preserved in README + git history) ([bdd67f3](https://github.com/teepean/bwa-mem3/commit/bdd67f3f77ad5bfbb46ef4041b632af7db66bba1))
* **install:** fix RHEL/Fedora package name pkgconfig → pkgconf-pkg-config ([#94](https://github.com/teepean/bwa-mem3/issues/94)) ([296b1b9](https://github.com/teepean/bwa-mem3/commit/296b1b9dae7533432060907dfe00d5c9007ad7e6))
* **install:** list autoconf/automake/libomp/zlib system prereqs ([#93](https://github.com/teepean/bwa-mem3/issues/93)) ([652ce0f](https://github.com/teepean/bwa-mem3/commit/652ce0f1ba371d9063bb5820aa62323d49ffd99e))
* pre-release documentation pass for v0.2.0-pre ([#96](https://github.com/teepean/bwa-mem3/issues/96)) ([3bc64b0](https://github.com/teepean/bwa-mem3/commit/3bc64b0df996386ad9af0953f4359e975119f379))
* **readme:** add bioconda badges and install instructions ([#106](https://github.com/teepean/bwa-mem3/issues/106)) ([830276c](https://github.com/teepean/bwa-mem3/commit/830276ce01774805c20bfff69c63cfebab239166))
* rename FG-MAIN.md to docs/whats-different.md ([34c8ea3](https://github.com/teepean/bwa-mem3/commit/34c8ea3be18c7b7610e4ee8fcfb065955e515a33))
* rewrite README for bwa-mem3 (lineage attribution, drop upstream-only sections) ([dddd8dd](https://github.com/teepean/bwa-mem3/commit/dddd8ddd8dbf147b0e974ba74a6b083ed26cb8ce))
* update whats-different.md for bwa-mem3 and main branch ([5719617](https://github.com/teepean/bwa-mem3/commit/5719617ca1daa49daff19265b5b22c63b6e6271b))
* **whats-different:** complete tables for v0.2.0 readiness ([#98](https://github.com/teepean/bwa-mem3/issues/98)) ([1e94a8e](https://github.com/teepean/bwa-mem3/commit/1e94a8ee5df8a16c480760c59835efedec78a4d0))

## [0.2.1](https://github.com/fg-labs/bwa-mem3/compare/v0.2.0...v0.2.1) (2026-05-17)


### Bug Fixes

* **changelog:** strip preamble so release-please owns the file ([#112](https://github.com/fg-labs/bwa-mem3/issues/112)) ([56e580c](https://github.com/fg-labs/bwa-mem3/commit/56e580cf4f2515280440b2882a32c3a6a7b6d15c))
* **mapq:** propagate SMEM SA-count to seed n_hits so --supp-rep-hard-cap works ([#101](https://github.com/fg-labs/bwa-mem3/issues/101)) ([cca9d4f](https://github.com/fg-labs/bwa-mem3/commit/cca9d4f41023e501636d2b1ebd2d1e825f95e8e3))
* **smem:** track enc_qdb byte capacity separately from wsize_mem ([#100](https://github.com/fg-labs/bwa-mem3/issues/100)) ([ab922b6](https://github.com/fg-labs/bwa-mem3/commit/ab922b6af531ed4521b6cd9bd3c43a661d51a421))


### Documentation

* **readme:** add bioconda badges and install instructions ([#106](https://github.com/fg-labs/bwa-mem3/issues/106)) ([830276c](https://github.com/fg-labs/bwa-mem3/commit/830276ce01774805c20bfff69c63cfebab239166))

## Changelog
