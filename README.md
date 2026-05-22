# WingSeek App Releases
Official releases for WingSeek, an app for bat survey video review and annotation.

➡️ **Download latest release:** [GitHub Releases](https://github.com/reeswag/WingSeek-App-Releases/releases)

WingSeek is a desktop app for bat survey video review, combining:
- Motion extraction
- AI prediction
- Event review and annotation
- Clip generation/export

Watch the WingSeek demo below with installation instructions and a full demonstration of the workflow:

[![Watch the WingSeek demo with installation instructions](https://img.youtube.com/vi/BAMXDqNjo84/hqdefault.jpg)](https://youtu.be/BAMXDqNjo84)

WingSeek is free to use. To support the project, please consider submitting clips to our database. These may be used to further improve the detection model. The upload link is available in the app.

If WingSeek has been useful to you and you would like to support ongoing updates, maintenance, and improvements, you can leave an optional contribution here:

➡️ [Support WingSeek](https://buymeacoffee.com/wingseek)

## Development Status

WingSeek has been developed and optimised for macOS and Linux.

The macOS app is fully optimised for Apple M-series CPU and GPU hardware. For optimal performance and the simplest user experience, please use the macOS release.

Windows and Linux versions are considered secondary releases. A GPU-enabled Linux release may be compiled directly from source code in future.

## Installation Instructions

### macOS

Use the bundled [Sentinel app](https://github.com/alienator88/Sentinel) to bypass Gatekeeper restrictions on macOS.

### Windows

Run as administrator. If a warning appears, click **More info**, then **Run anyway**.

### Linux

Double-click the `WingSeek` executable, or cd to the extracted directory and run `./WingSeek` from the terminal.

## Best Practices

WingSeek is non-destructive and does not modify the original input videos. However, we strongly recommend backing up all original survey videos prior to analysis.

WingSeek analyses input videos for motion and saves moving objects as small crops within the output directory.

It is important that the output directory:

1. Has sufficient free space.
2. Is on a sufficiently fast drive, so file writing does not cause slowdown.
3. Is not formatted as exFAT. Please use:
   - macOS: APFS
   - Windows: NTFS
   - Linux: ext4

Please select **Archive Outputs** from the main UI if you want to back up the output folder. This archives outputs into a `.tar` file for faster copying.

When analysis is complete and the Review UI has been used to generate clips, please ensure that the original videos are backed up alongside any clips containing bats.
