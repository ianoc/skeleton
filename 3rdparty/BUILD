java_plugin(
    name = "dagger_component_plugin",
    generates_api = 1,
    processor_class = "dagger.internal.codegen.ComponentProcessor",
    visibility = ["//visibility:public"],
    deps = [
        "@third_party_jvm//3rdparty/jvm/com/google/dagger",
        "@third_party_jvm//3rdparty/jvm/com/google/dagger:dagger_compiler",
        "@third_party_jvm//3rdparty/jvm/com/google/dagger:dagger_producers",
        "@third_party_jvm//3rdparty/jvm/com/google/dagger:dagger_spi",
    ],
)
