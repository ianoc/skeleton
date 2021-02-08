workspace(name = "skeleton")

BAZEL_VERSION = "4.0.0"
BAZEL_INSTALLER_VERSION_linux_SHA = "bd7a3a583a18640f58308c26e654239d412adaa833b6b6a7b57a216ab62fabc2"
BAZEL_INSTALLER_VERSION_darwin_SHA = "b4c94148f52854b89cff5de38a9eeeb4b0bcb3fb3a027330c46c468d9ea0898b"

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

http_archive(
    name = "com_google_protobuf",
    sha256 = "9748c0d90e54ea09e5e75fb7fac16edce15d2028d4356f32211cfa3c0e956564",
    strip_prefix = "protobuf-3.11.4",
    urls = ["https://github.com/protocolbuffers/protobuf/archive/v3.11.4.zip"],
)

load("@com_google_protobuf//:protobuf_deps.bzl", "protobuf_deps")
protobuf_deps()

load("//3rdparty:target_file.bzl", "build_external_workspace")
build_external_workspace("third_party_jvm")

load("//3rdparty:workspace.bzl", "maven_dependencies")
maven_dependencies()

