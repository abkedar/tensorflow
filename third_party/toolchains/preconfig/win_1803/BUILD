licenses(["restricted"])

package(default_visibility = ["//visibility:public"])

java_runtime(
    name = "windows_jdk8",
    srcs = [],
    java_home = "C:/openjdk",
)

platform(
    name = "rbe_windows_1803",
    constraint_values = [
        "@bazel_tools//platforms:x86_64",
        "@bazel_tools//platforms:windows",
    ],
    remote_execution_properties = """
        properties:{
          name:"container-image"
          value:"docker://gcr.io/tensorflow-testing/tf-rbe-win@sha256:b2eeb661e0134ef96a4736677e8f96a90970bc206dea93739cd711031b62a0e5"
        }
        properties:{
          name: "OSFamily" value: "Windows"
        }
        """,
)
