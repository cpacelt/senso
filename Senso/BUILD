load(
    "@rules_xcodeproj//xcodeproj:defs.bzl",
    "top_level_target",
    "xcodeproj",
)

load(
    "@build_bazel_rules_apple//apple:ios.bzl",
    "ios_application"
)

ios_application(
    name = "Senso",
    bundle_id = "rpts.senso",
    families = [
        "iphone",
        "ipad",
    ],
    minimum_os_version = "15.0",
    infoplists = ["Info.plist"],
    launch_storyboard = "Base.lproj/LaunchScreen.storyboard",
    visibility = [
        "//visibility:public",
    ],
    deps = [
        "//Modules/App:App",
    ],
)

xcodeproj(
    name = "xcodeproj",
    generation_mode = "incremental",
    project_name = "Senso",
    tags = ["manual"],
    top_level_targets = [
        top_level_target(":Senso", target_environments = ["simulator"]),
    ],
)
