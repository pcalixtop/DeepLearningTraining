load("@rules_cc//cc:defs.bzl", "cc_library")

cc_binary(
    name = "matrixApp",
    srcs = [
        "DeepLearningTrainingApp/app.cpp",
        "DeepLearningTrainingLib/matrix.cpp",
        "DeepLearningTrainingLib/matrix.h",
    ],
    deps = [":matriAppLib"],
)

cc_library(
    name = "matrixAppLib",
    srcs = [
        "DeepLearningTrainingLib/matrix.cpp",
        "DeepLearningTrainingLib/matrix.h",
    ],
)

cc_test(
    name = "matrixRowTest",
    srcs = [
        "DeepLearningTrainingUT/DeepLearningTrainingUT.cpp"
    ],
    deps = [
        "@com_google_googletest//:gtest_main",
        ":matrixAppLib",
    ],
)