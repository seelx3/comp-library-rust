---
data:
  _extendedDependsOn:
  - icon: ':heavy_check_mark:'
    path: rust/crates/helloworld/hello/src/lib.rs
    title: rust/crates/helloworld/hello/src/lib.rs
  - icon: ':heavy_check_mark:'
    path: rust/crates/helloworld/world/src/lib.rs
    title: rust/crates/helloworld/world/src/lib.rs
  - icon: ':heavy_check_mark:'
    path: rust/crates/io/input/src/lib.rs
    title: rust/crates/io/input/src/lib.rs
  - icon: ':warning:'
    path: rust/crates/io/scanner/src/lib.rs
    title: rust/crates/io/scanner/src/lib.rs
  _extendedRequiredBy: []
  _extendedVerifiedWith: []
  _isVerificationFailed: false
  _pathExtension: rs
  _verificationStatusIcon: ':warning:'
  attributes:
    links: []
  bundledCode: "Traceback (most recent call last):\n  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n          \
    \         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\
    \  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/languages/rust.py\"\
    , line 288, in bundle\n    raise NotImplementedError\nNotImplementedError\n"
  code: "//! Re-exports the crates for rustdoc.\n//!\n//! This crate itself is not\
    \ intended to be used directly.\n\n// With `custom-build` and `syn` crate, we\
    \ can expand crate-level rustdocs.\n\nmacro_rules! re_export(($($name:ident),*\
    \ $(,)?) => ($(pub mod $name { pub use ::$name::*; })*));\n\npub mod helloworld\
    \ {\n    //! Crates of \"hello\" and \"world\".\n\n    re_export!(hello, world);\n\
    }\n\npub mod io {\n    //! Crates about IO.\n\n    re_export!(input, scanner);\n\
    }\n"
  dependsOn:
  - rust/crates/helloworld/hello/src/lib.rs
  - rust/crates/helloworld/world/src/lib.rs
  - rust/crates/io/input/src/lib.rs
  - rust/crates/io/scanner/src/lib.rs
  isVerificationFile: false
  path: rust/src/lib.rs
  requiredBy: []
  timestamp: '2023-02-04 17:04:39+00:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: rust/src/lib.rs
layout: document
redirect_from:
- /library/rust/src/lib.rs
- /library/rust/src/lib.rs.html
title: rust/src/lib.rs
---
