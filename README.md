Quick start examples for [Banuba SDK on Android](https://docs.banuba.com/face-ar-sdk-v1/android/android_overview) and [Agora.io](https://www.agora.io/en/) SDK integration to enhance video calls with real-time face filters and virtual backgrounds.  
  
# Getting Started

1. Visit agora.io to sign up and get token, app and channel ID
2. Copy and Paste your agora token, app and chanel ID into appropriate section of `videocall-android-kotlin/app/src/main/java/com/banuba/sdk/example/videocall/AgoraClientToken.kt` with “” symbols. For example: agora_token = “place_your_token_here”
3. Open the project in Android Studio and run the necessary target using the usual steps.

# How an example works

This project is based on the BanubaSDKManager. BanubaSdkManager creates and manages the Banuba camera. Agor also has its own camera module, but in this example the Agora camera is not used, so in order to disable Agora camera is called setExternalVideoSource(...).  The frames from the Banuba camera are processed within BanubaSdk and the result transferred to the handler onFrameRendered(...). In the handler, frames are passed to the Agora module via pushExternalVideoFrame(...).

# Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
