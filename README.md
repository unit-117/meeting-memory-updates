# Meeting Memory for macOS

Native meeting audio capture, local transcripts, and in-app updates.

## Download

[Download Meeting Memory 0.3.0](https://github.com/unit-117/meeting-memory-updates/releases/download/v0.3.0/MeetingMemory-0.3.0.zip)

Requires macOS 15 or later on Apple silicon. See [release notes](https://github.com/unit-117/meeting-memory-updates/releases/tag/v0.3.0).

## Install

Quit Meeting Memory, unzip the download, and move **Meeting Memory.app** into Applications. If you have an older test version, replace it once. Existing recordings and settings remain in their existing locations. macOS may ask for permissions again when moving from an unsigned test build to the signed release.

After that, use **Meeting Memory → Check for Updates**. Update installation waits for recording, transcription, and delivery to finish. The app verifies signed update information and downloads.

## More than one Mac

Use the same download on each Apple silicon Mac running macOS 15 or later. No developer account or signing certificate is needed on the receiving computers. Grant recording and speech permissions separately on each Mac; each installation checks the same update feed.

Recordings and transcripts are stored locally on the Mac that captured them. The installer does not sync libraries or copy your ChatGPT connection. Optional ChatGPT delivery needs separate private setup on each Mac, including checking the current delivery helper's Python 3 requirement.

Obtain participant consent before recording. Check the complete workflow with a short consenting test call after installation.

This repository contains distribution files only. App source code, recordings, transcripts, account credentials, and private signing keys are not stored here.
