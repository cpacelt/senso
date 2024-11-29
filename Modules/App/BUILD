load(
    "@build_bazel_rules_apple//apple:ios.bzl",
    "ios_application"
)

load(
    "@build_bazel_rules_swift//swift:swift.bzl",
    "swift_library"
)

swift_library(
    name = "App",
    module_name = "App",
    srcs = glob([
         "Sources/**/*.swift",
    ]),
    visibility = [
        "//visibility:public",
    ],
)
