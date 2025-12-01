# FluidVoice

Voice-to-text dictation app for macOS with AI enhancement.

## Features

- Real-time transcription using Parakeet TDT v2 model (English)
- Live preview overlay with notch support
- Command Mode for system control
- Write Mode for typing into any app
- AI enhancement with OpenAI, Groq, and custom providers
- Global hotkey support
- Menu bar integration

## Recent Changes

- Fix caching issue in ASR service
- Moved overlay UI to the bottom
- Updated to English-only v2 model

## Requirements

- macOS 14.0 (Sonoma) or later
- Apple Silicon Mac (M1, M2, M3, M4)

## Build for Production

```bash
git clone https://github.com/EliseiNicolae/FluidVoice.git
cd FluidVoice

xcodebuild -project Fluid.xcodeproj -scheme Fluid -configuration Release -derivedDataPath ./build clean build

cp -R ./build/Build/Products/Release/Fluid.app /Applications/
```

## License

[Apache License 2.0](LICENSE)
