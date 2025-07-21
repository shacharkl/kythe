package(default_visibility = ["//visibility:public"])

load("//:setup.bzl", "kythe_visibility_groups")
load("//:external_visibility.bzl", "EXTERNAL_VISIBILITY")
kythe_visibility_groups(external_visibility = EXTERNAL_VISIBILITY)

filegroup(
    name = "srcs",
    srcs = glob(
        ["**"],
        exclude = [
            "web/site/.bundle/**",
            "web/site/_vendor/**",
        ],
    ),
    visibility = ["//visibility:private"],
)
