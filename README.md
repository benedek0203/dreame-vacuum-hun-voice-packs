<h1 align="center">Dreame Vacuum Hungarian Voice Packs</h1>

Enhance your Dreame vacuum cleaner with a custom Hungarian voice packs. Enjoy voice notifications in the Hungarian language for cleaning progress, battery status, cleaning scheduling, errors, and more.

## 💡Introduction

First I would like to say thanks to Oleksandr Belei for inspiration and for this ReadMe.

Since the official Dreame app lacks native Hungarian language support, this project was created to provide Hungarian voice packs for your Dreame vacuum cleaner. These voice packs are created using paid AI voice generation services and then fine-tuned with Audacity to ensure quality audio output.

## 🚀Features

**Available Voice Packs:**

| Voice Pack                  | Description                    | Hash                               | Size      | Samples                                         |
| --------------------------- | ------------------------------ | ---------------------------------- | --------- | ----------------------------------------------- |
| [voice](voice_packs/voice/) | _Harsh, aggressive and vulgar_ | `bcccfef6ad2843586c80857d2983f6e8` | `4391337` | <p align="center">[🔗](voice_samples/voice)</p> |

## ⚙️Installation

You can install the Hungarian voice pack on your Dreame vacuum cleaner using one of the following methods:

### 1. Installing on Official Firmware with [Home Assistant](https://www.home-assistant.io/)

- Install the custom [Dreame vacuum](https://github.com/Tasshack/dreame-vacuum.git) integration for Home Assistant, created by **@Tasshack**.
- In Home Assistant, navigate to `"Developer Tools"` -> `"Actions"` and select action `Dreame Vacuum: Install Voice Pack`.

  - Targets: Choose entity -> select your robot
  - Language ID: RU (or can be EN, but it was not working for me)
  - URL: Raw URL for the voice pack from the "voice_packs" directory in this repository. (
    https://github.com/benedek0203/dreame-vacuum-hun-voice-packs/raw/refs/heads/main/voice_packs/voice.tar.gz)
  - MD5: The hash of the voice pack. (bcccfef6ad2843586c80857d2983f6e8)
  - Size: The file size of the voice pack in bytes. (4391337)

- Call the service to set the new voice pack.

### 2. Installing on Custom Firmware with [Valetudo](https://valetudo.cloud/)

- Open Valetudo's web interface by entering your vacuum's IP address in a web browser.
- In Valetudo, navigate to `"Robot Settings"`-> `"Misc Settings."`
- Enter the following information in the `"Voice packs"` section:
  - **URL:** Raw URL for the voice pack from the "voice_packs" directory in this repository.
  - **Language Code:** 'UK'
  - **Hash:** The hash of the voice pack.
  - **File size:** The file size of the voice pack in bytes.
- Save the settings by clicking `"Set Voice Pack`."

### 3. Installing on Official Firmware with [Python MIIO](https://python-miio.readthedocs.io/en/latest/)

Detailed installation instructions can be found in the [python-miio](https://github.com/rytilahti/python-miio.git) repository, created by **@rytilahti**.

## 📜License

This project is open-source and available under the [MIT License](LICENSE). You are free to use and modify it as per the terms of the license.

## 💬Discussions

If you have any questions, suggestions, or feedback, please visit the [Discussion](../../discussions) tab of this repository. Feel free to start a new discussion or join existing ones.

---

❗**Disclaimer:** This project is not affiliated with or endorsed by Dreame or its parent companies. It is an independent, community-driven effort to provide custom voice packs for Dreame Vacuum Cleaners.
