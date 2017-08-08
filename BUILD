config_setting(
    name = "linux_x86_64",
    values = {"cpu": "k8"},
    visibility = ["//visibility:public"],
)

config_setting(
    name = "windows",
    values = {"cpu": "x64_windows"},
    visibility = ["//visibility:public"],
)

cc_binary(
    name="python-test",
    srcs = [
        "main.c",
    ],
    deps = select({
        "//:linux_x86_64": [
            "@python_linux//:python35-lib"
        ],
        "//:windows": [
            "@python_win//:python35-lib"
        ]
    })
)
