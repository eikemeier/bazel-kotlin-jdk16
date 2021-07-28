workspace(name = "com_example_bazel_kotlin_jdk16")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_android",
    sha256 = "6461c1c5744442b394f46645957d6bd3420eb1b421908fe63caa03091b1b3655",
    strip_prefix = "rules_android-0.1.1",
    urls = ["https://github.com/bazelbuild/rules_android/archive/refs/tags/v0.1.1.tar.gz"],
)

http_archive(
    name = "io_bazel_rules_kotlin",
    sha256 = "58edd86f0f3c5b959c54e656b8e7eb0b0becabd412465c37a2078693c2571f7f",
    url = "https://github.com/bazelbuild/rules_kotlin/releases/download/v1.5.0-beta-3/rules_kotlin_release.tgz",
)

load("@io_bazel_rules_kotlin//kotlin:repositories.bzl", "kotlin_repositories")
load("@io_bazel_rules_kotlin//kotlin:kotlin.bzl", "kt_register_toolchains")

kotlin_repositories()

kt_register_toolchains()
