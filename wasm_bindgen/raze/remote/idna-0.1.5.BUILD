"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""
package(default_visibility = [
  # Public for visibility by "@raze__crate__version//" targets.
  #
  # Prefer access through "//wasm_bindgen/raze", which limits external
  # visibility to explicit Cargo.toml dependencies.
  "//visibility:public",
])

licenses([
  "notice", # "MIT,Apache-2.0"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_library",
    "rust_binary",
    "rust_test",
)



rust_library(
    name = "idna",
    crate_root = "src/lib.rs",
    crate_type = "lib",
    edition = "2015",
    srcs = glob(["**/*.rs"]),
    deps = [
        "@raze__matches__0_1_8//:matches",
        "@raze__unicode_bidi__0_3_4//:unicode_bidi",
        "@raze__unicode_normalization__0_1_8//:unicode_normalization",
    ],
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.1.5",
    crate_features = [
    ],
)

# Unsupported target "tests" with type "test" omitted
# Unsupported target "unit" with type "test" omitted