---
data:
  _extendedDependsOn: []
  _extendedRequiredBy:
  - icon: ':heavy_check_mark:'
    path: rust/crates/io/input/src/lib.rs
    title: rust/crates/io/input/src/lib.rs
  - icon: ':warning:'
    path: rust/src/lib.rs
    title: rust/src/lib.rs
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
  code: "//! A quite simple input scanner.\n//!\n//! ```no_run\n//! use scanner::Scanner;\n\
    //!\n//! let mut sc = Scanner::from_stdin();\n//! let _: u64 = sc.read();\n//!\
    \ ```\n\nuse std::{\n    any, fmt,\n    io::{self, Read as _},\n    str::{FromStr,\
    \ SplitAsciiWhitespace},\n};\n\n/// A quite simple input scanner.\npub struct\
    \ Scanner {\n    tokens: SplitAsciiWhitespace<'static>,\n}\n\nimpl Scanner {\n\
    \    /// Constructs a new `Self` with while input from stdin.\n    ///\n    ///\
    \ # Panics\n    ///\n    /// Panics if an IO error occurred.\n    pub fn from_stdin()\
    \ -> Self {\n        let mut input = \"\".to_owned();\n        io::stdin().read_to_string(&mut\
    \ input).unwrap();\n        Self {\n            tokens: Box::leak(input.into_boxed_str()).split_ascii_whitespace(),\n\
    \        }\n    }\n\n    /// Consumes and parses the next token.\n    ///\n  \
    \  /// # Panics\n    ///\n    /// Panics if:\n    ///\n    /// - no token left\n\
    \    /// - failed to parse the token\n    pub fn read<T>(&mut self) -> T\n   \
    \ where\n        T: FromStr,\n        T::Err: fmt::Display,\n    {\n        let\
    \ token = self.tokens.next().expect(\"reached EOF\");\n        token.parse().unwrap_or_else(|err|\
    \ {\n            panic!(\n                \"could not parse {:?} as `{}`: {}\"\
    ,\n                token,\n                any::type_name::<T>(),\n          \
    \      err,\n            );\n        })\n    }\n}\n"
  dependsOn: []
  isVerificationFile: false
  path: rust/crates/io/scanner/src/lib.rs
  requiredBy:
  - rust/src/lib.rs
  - rust/crates/io/input/src/lib.rs
  timestamp: '2023-02-04 17:04:39+00:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: rust/crates/io/scanner/src/lib.rs
layout: document
redirect_from:
- /library/rust/crates/io/scanner/src/lib.rs
- /library/rust/crates/io/scanner/src/lib.rs.html
title: rust/crates/io/scanner/src/lib.rs
---
