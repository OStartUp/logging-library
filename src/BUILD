#https://www.python.org/ftp/python/3.7.6/Python-3.7.6.tgz
package(default_visibility = ["//visibility:public"]) 
load("@rules_python//python:pip.bzl", "pip_import")



py_library(
    name = "logger",
    srcs = ["logger.py"],
    srcs_version = "PY3",
    imports= ["config"],
    deps = ["@config//src:config"],
)




py_binary(
    name = "dummy",
    srcs = ["dummy.py"],
    srcs_version = "PY3",
    imports= ["config"],
    deps = [":logger", "@config//src:config"], 
)

# config_pkg
# config-wheel
# config