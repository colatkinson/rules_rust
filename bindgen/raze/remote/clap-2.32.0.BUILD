"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""

package(default_visibility = [
    # Public for visibility by "@raze__crate__version//" targets.
    #
    # Prefer access through "//bindgen/raze", which limits external
    # visibility to explicit Cargo.toml dependencies.
    "//visibility:public",
])

licenses([
    "notice",  # "MIT"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_binary",
    "rust_library",
    "rust_test",
)

rust_library(
    name = "clap",
    srcs = glob(["**/*.rs"]),
    crate_features = [
        "ansi_term",
        "atty",
        "color",
        "default",
        "strsim",
        "suggestions",
        "vec_map",
    ],
    crate_root = "src/lib.rs",
    crate_type = "lib",
    edition = "2015",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "2.32.0",
    deps = [
        "@raze__ansi_term__0_11_0//:ansi_term",
        "@raze__atty__0_2_11//:atty",
        "@raze__bitflags__1_0_4//:bitflags",
        "@raze__strsim__0_7_0//:strsim",
        "@raze__textwrap__0_10_0//:textwrap",
        "@raze__unicode_width__0_1_5//:unicode_width",
        "@raze__vec_map__0_8_1//:vec_map",
    ],
)
