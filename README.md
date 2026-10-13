# Dictation

Turn voice recordings from your phone into text on your own computer. You can also translate
the text and save it as a Word document, a PDF or a text file.

Everything runs on your computer. Your recordings aren't uploaded anywhere, unless you choose
the Google Translate option.

## Download

| Your computer | Download |
|---|---|
| Windows 10 or 11 | [Dictation-Windows.zip](https://github.com/JakeC137/dictation-download/releases/latest/download/Dictation-Windows.zip) |
| Mac with an Apple chip (M1, M2, M3, M4) | [Dictation-Mac-AppleSilicon.zip](https://github.com/JakeC137/dictation-download/releases/latest/download/Dictation-Mac-AppleSilicon.zip) |
| Mac with an Intel processor | [Dictation-Mac-Intel.zip](https://github.com/JakeC137/dictation-download/releases/latest/download/Dictation-Mac-Intel.zip) |

Not sure which Mac you have? Click the Apple menu → *About This Mac*. It says *Chip: Apple M…*
or *Processor: … Intel …*.

## Install on Windows

1. Right-click the downloaded zip → **Extract All**.
2. Open the **Dictation** folder and double-click **Dictation.exe**.

The first time, Windows may show two messages:

- *"Windows protected your PC"*: click **More info → Run anyway**. This appears because the
  program comes from a person, not a company.
- A question about network access: allow **Private networks**, so your phone can connect.

## Install on a Mac

You need macOS 14 (Sonoma) or newer.

1. Double-click the downloaded zip, then drag **Dictation** into your *Applications* folder.
2. Double-click **Dictation**.
3. The first time, macOS blocks it, because it isn't from the App Store or a registered
   developer:
   1. Click **Done**.
   2. Open **System Settings → Privacy & Security**, scroll down, and click **Open Anyway**
      next to *"Dictation" was blocked*.
   3. Confirm with your password.
4. If asked whether Dictation may accept incoming network connections, click **Allow**, so your
   phone can connect.

If macOS says Dictation *"is damaged and can't be opened"*, open *Terminal*, type the following
command and press Return, then try again:

```
xattr -cr /Applications/Dictation.app
```

## First start

A small **Dictation** window appears and Dictation opens in your web browser. **Closing that
window stops Dictation.**

The first time, Dictation downloads its speech recognition and translation models. That's
about 3 GB, plus 1.4 GB on PCs with an NVIDIA graphics card. The page shows the progress, and
it only happens once.

## Use it with your phone

1. Make sure your phone is on the same Wi-Fi as the computer.
2. Scan the QR code on the Dictation page with your phone's camera.
3. Tap **Choose a recording** and pick the audio file:
   - **iPhone:** in Voice Memos, tap the recording → ••• → *Save to Files* first, then choose
     it from *Browse*.
   - **Android:** pick it from *Recordings*, *Audio* or your file manager.

You can also drag a file from the computer onto the page.

When the transcript is ready, you can:

- Correct it.
- Translate it into about 100 languages.
- Download it as TXT, Word or PDF.

## Uninstall

Delete the program, then delete these folders:

- **Windows:**
  - `%LOCALAPPDATA%\Dictation` (paste this into the File Explorer address bar)
  - `Documents\Dictation`
- **Mac:**
  - `~/Library/Application Support/Dictation` (in Finder: *Go → Go to Folder…*)
  - `Documents/Dictation`

The translation model (NLLB-200 by Meta) may only be used for non-commercial purposes.
