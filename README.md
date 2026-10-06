# Meeting Memory for macOS

Native meeting audio capture, local transcripts, and in-app updates.

## Download

[Download Meeting Memory 0.3.4](https://github.com/unit-117/meeting-memory-updates/releases/download/v0.3.4/MeetingMemory-0.3.4.zip)

Requires macOS 15 or later on Apple silicon. See [release notes](https://github.com/unit-117/meeting-memory-updates/releases/tag/v0.3.4).

## Install

Quit Meeting Memory, unzip the download, and move **Meeting Memory.app** into Applications. If you have an older test version, replace it once. Existing recordings and settings remain in their existing locations. macOS may ask for permissions again when moving from an unsigned test build to the signed release.

After that, use **Meeting Memory → Check for Updates**. Update installation waits for recording, transcription, and delivery to finish. The app verifies signed update information and downloads.

## More than one Mac

Use the same download on each Apple silicon Mac running macOS 15 or later. No developer account or signing certificate is needed on the receiving computers. Grant recording and speech permissions separately on each Mac; each installation checks the same update feed.

Recordings and transcripts are stored locally on the Mac that captured them. The installer does not sync libraries or copy your ChatGPT connection. Optional ChatGPT delivery needs separate private setup on each Mac, including checking the current delivery helper's requirement for a working `/usr/bin/python3`.

Obtain participant consent before recording. Check the complete workflow with a short consenting test call after installation.

This repository contains distribution files only. App source code, recordings, transcripts, account credentials, and private signing keys are not stored here.

## Delivery and capture checks

ChatGPT uploads are paced at one part every 90 seconds. Keep the Mac awake until pending uploads finish; an interrupted upload resumes when the app next runs. Uploaded means the cloud accepted the content, not that the final Pages have been verified. Check your Meetings space, and use the meeting menu’s **Retry saving in ChatGPT** if a part is missing. Exact exports remain private on the source Mac for recovery.

Silent meeting audio now shows a warning. Microphone and meeting-audio labels identify tracks, not people. Validate audible remote participants in a consenting call; a Ready transcript alone is not evidence that both sides were captured.
