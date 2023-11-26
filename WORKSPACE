workspace(name = "com_github_storypku_rules_folly")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("//bazel:folly_deps.bzl", "folly_deps")

folly_deps(with_gflags = 1)

load("@com_github_nelhage_rules_boost//:boost/boost.bzl", "boost_deps")

boost_deps()

http_archive(
    name = "com_google_googletest",
    sha256 = "b4870bf121ff7795ba20d20bcdd8627b8e088f2d1dab299a031c1034eddc93d5",
    strip_prefix = "googletest-release-1.11.0",
    urls = [
        "https://github.com/google/googletest/archive/release-1.11.0.tar.gz",
    ],
)

http_archive(
    name = "com_github_3rdparty_bazel_rules_libevent",
    sha256 = "b4870bf121ff7795ba20d20bcdd8627b8e088f2d1dab299a031c1034eddc93d5",
    strip_prefix = "bazel-rules-libevent-58f892d39007a50452f78bab7fa6c5756b8e02eb",
    urls = [
        "https://github.com/3rdparty/bazel-rules-libevent/archive/58f892d39007a50452f78bab7fa6c5756b8e02eb.zip",
    ],
)

load("@com_github_3rdparty_bazel_rules_libevent//bazel:repos.bzl", libevent_repos="repos")
libevent_repos()

load("@com_github_3rdparty_bazel_rules_libevent//bazel:deps.bzl", libevent_deps="deps")
libevent_deps()
