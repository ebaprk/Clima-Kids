# Clima Kids

A SwiftUI educational app that introduces climate change through short learning stages and a quiz. It is packaged as a Swift Playgrounds iOS app project.

## Features

- Separate Learn and Quiz sections.
- Staged educational content with reusable navigation and header components.
- A Combine-based quiz service that tracks answers, score, and progress.
- Bundled artwork and audio, with Subsonic for sound playback.

## Requirements and setup

- A Mac or iPad with Swift Playgrounds capable of opening iOS app projects, or a compatible Xcode installation.
- The manifest targets iOS 15.2 or later and declares Swift tools 5.6.
- Internet access for the Subsonic Swift package dependency.

```sh
git clone https://github.com/ebaprk/Clima-Kids.git
cd Clima-Kids
```

Open the app package with Swift Playgrounds. If the downloaded folder is not recognized as an app playground, use a working copy with the `.swiftpm` extension and open it in Swift Playgrounds. The manifest imports `AppleProductTypes`; this is an Apple app project, so a plain command-line `swift run` is not the intended launch path. Use your own signing team and bundle identifier when running on a device.

## Project guide

| Location | Purpose |
| --- | --- |
| [Package.swift](Package.swift) | App product, supported devices, resources, and dependency. |
| [MainView.swift](MainView.swift) | Top-level Learn/Quiz navigation. |
| [Learn/](Learn/) | Learning stages and their view model. |
| [Quiz/](Quiz/) | Quiz interface, question model, and Combine service. |
| [Resources/](Resources/) | Bundled audio. |

## License

[MIT](LICENSE). Third-party packages retain their own licenses.
