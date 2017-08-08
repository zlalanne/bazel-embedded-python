new_local_repository(
    name = "python_linux",
    path = "/usr",
    build_file_content = """
cc_library(
    name = "python35-lib",
    srcs = ["lib/python3.5/config-3.5m-x86_64-linux-gnu/libpython3.5.so"],
    hdrs = glob(["include/python3.5/*.h"]),
    includes = ["include/python3.5"],
    visibility = ["//visibility:public"]
)
    """
)

new_local_repository(
    name = "python_win",
    path = "C:/Python35",
    build_file_content = """
cc_library(
    name = "python35-lib",
    srcs = ["libs/python35.lib"],
    hdrs = glob(["include/*.h"]),
    includes = ["include/"],
    visibility = ["//visibility:public"]
)
    """
)
