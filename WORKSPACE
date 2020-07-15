workspace(name = "gamester_ios")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "build_bazel_rules_apple",
    sha256 = "7a7afdd4869bb201c9352eed2daf37294d42b093579b70423490c1b4d4f6ce42",
    url = "https://github.com/bazelbuild/rules_apple/releases/download/0.19.0/rules_apple.0.19.0.tar.gz",
)

load(
    "@build_bazel_rules_apple//apple:repositories.bzl",
    "apple_rules_dependencies",
)

apple_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()

load(
    "@build_bazel_apple_support//lib:repositories.bzl",
    "apple_support_dependencies",
)

apple_support_dependencies()

load(
    "@com_google_protobuf//:protobuf_deps.bzl",
    "protobuf_deps",
)

protobuf_deps()

http_archive(
   name = "CNIOLinux",
   url = "https://github.com/apple/swift-nio/archive/2.19.0.tar.gz",
   strip_prefix = "swift-nio-2.19.0",
   build_file = "@//:Pods/CNIOLinux/BUILD"
)

http_archive(
   name = "Rx",
   url = "https://github.com/ReactiveX/RxSwift/archive/4.2.0.tar.gz",
   strip_prefix = "RxSwift-4.2.0",
   sha256 = "d8474e9733075e7164732b25284c263d0b16e9c9a18393de932bd8ddded73360",
   build_file = "@//:Pods/RxSwift/BUILD"
)
