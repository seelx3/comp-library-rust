---
data:
  _extendedDependsOn:
  - icon: ':warning:'
    path: rust/crates/io/scanner/src/lib.rs
    title: rust/crates/io/scanner/src/lib.rs
  _extendedRequiredBy:
  - icon: ':warning:'
    path: rust/src/lib.rs
    title: rust/src/lib.rs
  _extendedVerifiedWith:
  - icon: ':heavy_check_mark:'
    path: rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs
    title: rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs
  - icon: ':heavy_check_mark:'
    path: rust/verification/src/bin/library-checker-aplusb.rs
    title: rust/verification/src/bin/library-checker-aplusb.rs
  _isVerificationFailed: false
  _pathExtension: rs
  _verificationStatusIcon: ':heavy_check_mark:'
  attributes:
    links: []
  bundledCode: "Traceback (most recent call last):\n  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n          \
    \         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\
    \  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/languages/rust.py\"\
    , line 288, in bundle\n    raise NotImplementedError\nNotImplementedError\n"
  code: "//! A limited `input!` macro.\n//!\n//! ```no_run\n//! use input::input;\n\
    //!\n//! input! {\n//!     a: u32,\n//!     b: u32,\n//! }\n//! ```\n\npub use\
    \ scanner::Scanner;\n\n/// A limited `input!` macro.\n#[macro_export]\nmacro_rules!\
    \ input {\n    ($($var:ident : $ty:ty),* $(,)?) => {\n        let mut __scanner\
    \ = $crate::Scanner::from_stdin();\n        $(\n            let $var = __scanner.read::<$ty>();\n\
    \        )*\n    };\n}\n"
  dependsOn:
  - rust/crates/io/scanner/src/lib.rs
  isVerificationFile: false
  path: rust/crates/io/input/src/lib.rs
  requiredBy:
  - rust/src/lib.rs
  timestamp: '2023-02-04 17:04:39+00:00'
  verificationStatus: LIBRARY_ALL_AC
  verifiedWith:
  - rust/verification/src/bin/library-checker-aplusb.rs
  - rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs
documentation_of: rust/crates/io/input/src/lib.rs
layout: document
redirect_from:
- /library/rust/crates/io/input/src/lib.rs
- /library/rust/crates/io/input/src/lib.rs.html
title: rust/crates/io/input/src/lib.rs
---
