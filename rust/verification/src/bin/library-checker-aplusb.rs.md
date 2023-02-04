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
  _extendedRequiredBy: []
  _extendedVerifiedWith: []
  _isVerificationFailed: false
  _pathExtension: rs
  _verificationStatusIcon: ':heavy_check_mark:'
  attributes:
    PROBLEM: https://judge.yosupo.jp/problem/aplusb
    links:
    - https://judge.yosupo.jp/problem/aplusb
  bundledCode: "Traceback (most recent call last):\n  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n          \
    \         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\
    \  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/languages/rust.py\"\
    , line 288, in bundle\n    raise NotImplementedError\nNotImplementedError\n"
  code: "// verification-helper: PROBLEM https://judge.yosupo.jp/problem/aplusb\n\n\
    use input::input;\n\nfn main() {\n    input! {\n        a: u32,\n        b: u32,\n\
    \    }\n\n    println!(\"{}\", a + b);\n}\n"
  dependsOn:
  - rust/crates/helloworld/hello/src/lib.rs
  - rust/crates/helloworld/world/src/lib.rs
  - rust/crates/io/input/src/lib.rs
  isVerificationFile: true
  path: rust/verification/src/bin/library-checker-aplusb.rs
  requiredBy: []
  timestamp: '2023-02-04 17:04:39+00:00'
  verificationStatus: TEST_ACCEPTED
  verifiedWith: []
documentation_of: rust/verification/src/bin/library-checker-aplusb.rs
layout: document
redirect_from:
- /verify/rust/verification/src/bin/library-checker-aplusb.rs
- /verify/rust/verification/src/bin/library-checker-aplusb.rs.html
title: rust/verification/src/bin/library-checker-aplusb.rs
---
