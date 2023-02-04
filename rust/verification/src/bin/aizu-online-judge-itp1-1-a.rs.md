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
    PROBLEM: http://judge.u-aizu.ac.jp/onlinejudge/description.jsp?id=ITP1_1_A
    links:
    - http://judge.u-aizu.ac.jp/onlinejudge/description.jsp?id=ITP1_1_A
  bundledCode: "Traceback (most recent call last):\n  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n          \
    \         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\
    \  File \"/opt/hostedtoolcache/Python/3.11.1/x64/lib/python3.11/site-packages/onlinejudge_verify/languages/rust.py\"\
    , line 288, in bundle\n    raise NotImplementedError\nNotImplementedError\n"
  code: "// verification-helper: PROBLEM http://judge.u-aizu.ac.jp/onlinejudge/description.jsp?id=ITP1_1_A\n\
    \nfn main() {\n    println!(\"{} {}\", hello::HELLO, world::WORLD);\n}\n"
  dependsOn:
  - rust/crates/helloworld/hello/src/lib.rs
  - rust/crates/helloworld/world/src/lib.rs
  - rust/crates/io/input/src/lib.rs
  isVerificationFile: true
  path: rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs
  requiredBy: []
  timestamp: '2023-02-04 17:04:39+00:00'
  verificationStatus: TEST_ACCEPTED
  verifiedWith: []
documentation_of: rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs
layout: document
redirect_from:
- /verify/rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs
- /verify/rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs.html
title: rust/verification/src/bin/aizu-online-judge-itp1-1-a.rs
---
