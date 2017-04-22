
android_library(
    name = "activities",
    srcs = glob(["app/src/main/java/**/*.java"]),
    custom_package = "com.example.bazel_aar_test",
    manifest = "app/src/main/AndroidManifest.xml",
    resource_files = glob(["app/src/main/res/**"]),
    deps = [
        "@androidsdk//com.android.support:support-compat-25.3.1",
        "@androidsdk//com.android.support:appcompat-v7-25.3.1",
        "@androidsdk//com.android.support:design-25.3.1",
        "@androidsdk//com.android.support:percent-25.3.1",
        "@androidsdk//com.android.support:recyclerview-v7-25.3.1",
        ],
)
android_binary(
    name = "bazel_aar_test",
    custom_package = "com.example.bazel_aar_test",
    manifest = "app/src/main/AndroidManifest.xml",
    deps = [
        ":activities",
        "@androidsdk//com.android.support:support-compat-25.3.1",
        "@androidsdk//com.android.support:appcompat-v7-25.3.1",
        "@androidsdk//com.android.support:design-25.3.1",
        "@androidsdk//com.android.support:percent-25.3.1",
        "@androidsdk//com.android.support:recyclerview-v7-25.3.1",
        "@android_image_cropper//aar",
    ],
)