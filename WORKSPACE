load("/WORKSPACE.user", "android_sdk_path", "android_ndk_path")
load("@bazel_tools//tools/build_defs/repo:maven_rules.bzl", "maven_aar")

android_sdk_repository(
    name = "androidsdk",
    path = android_sdk_path(),
    api_level = 25,
    build_tools_version = "25.0.2",
)

android_ndk_repository(
    name = "androidndk",
    path = android_ndk_path(),
    api_level = 19,
)

maven_aar(
    name = "android_image_cropper", 
    artifact = "com.theartofdev.edmodo:android-image-cropper:2.3.1",
    settings = "//:maven_settings.xml")
