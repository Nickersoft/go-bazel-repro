load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

ODICT_VERSION = "d2a405a2187dcd11f6a2ef46640e87bb161537bc"

http_archive(
    name = "odict",
    sha256 = "70113fae902be6b1da8bb79ac9c6a2854c6e0d2196503531e2908f021a676ae7",
    strip_prefix = "odict-%s" % ODICT_VERSION,
    url = "https://github.com/TheOpenDictionary/odict/archive/%s.tar.gz" % ODICT_VERSION,
)

load("@odict//bazel:odict_deps.bzl", "odict_deps")

odict_deps()

load("@odict//bazel:odict_extra_deps.bzl", "odict_extra_deps")

odict_extra_deps()
