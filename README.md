# Every Day Wear
In this repo, we integrate Vuzix Z100 with iOS to create a variety of functionality geared towards the AR glasses use case of every-day wear.

This repo is based on the [Ultralite SDK Sample for iOS application](https://github.com/Vuzix/ultralite-sdk-ios-sample) built using the [Ultralite SDK for iOS](https://github.com/Vuzix/UltraliteSDK-releases-iOS). 

## Simple Timer

## How to Use
Click the "Create Hello World" button to trigger `startSpeechRecognition` (in `ViewController`). Voice input: "Set a `n` minute timer."

## How It Works
This phrase is passed to a llama-3.1-8B model (hosted on [build.nvidia.com](https://build.nvidia.com/meta/llama-3_1-8b-instruct)). You may have to change the `apiKey` variable in the `parseTimerCommand` function.

The LLM extracts the key number `n` and sets an `n` minute timer, which is displayed counting down on the Vuzix display. When the timer finishes, the words "Time's up!" is displayed and the app also sends a notification.

## Other ideas
GPT wrapper
add to notes
add to calendar
send message (text, discord)
Spotify? How to design to see full playlist



