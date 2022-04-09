load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

ODICT_VERSION = "1.4.6"

http_archive(
    name = "odict",
    sha256 = "26f78f1ef1fd1e3603362a5fe7d945a2033c2e0fa2a79e852f908c51bcf2b97c",
    strip_prefix = "odict-%s" % ODICT_VERSION,
    url = "https://github.com/TheOpenDictionary/odict/archive/refs/tags/%s.tar.gz" % ODICT_VERSION,
)

load("@odict//bazel:odict_deps.bzl", "odict_deps")

odict_deps()

load("@odict//bazel:odict_extra_deps.bzl", "odict_extra_deps")

odict_extra_deps()
