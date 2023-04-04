![Release](https://img.shields.io/github/v/release/jczic/ESP32-MPY-Jama?include_prereleases&color=success)
![Windows 64bits](https://img.shields.io/badge/Windows_64bits-Ok-green.svg)
![MacOS ARM64](https://img.shields.io/badge/MacOS_ARM64-Ok-green.svg)
![MacOS Intel x86_64](https://img.shields.io/badge/MacOS_Intel_x86__64-Ok-green.svg)
![License](https://img.shields.io/github/license/jczic/ESP32-MPY-Jama?color=yellow)

# <img src="/img/logo.png" width="45" valign="bottom">  ESP32 MPY-Jama v1.2, the dev tool for your favorite MCU

### <p align="justify">A powerful tool that easily connects to Espressif ESP32 microcontrollers with MicroPython, providing an IDE, file manager, REPL, real time dashboards and advanced features for efficient development on MacOS, Windows and Linux.</p>

<br />

<p align="center">
    <img src="/img/screen-ide.png" width="700">
</p>

<h4>
    <p align="center">
        MacOS on arm64 / MacOS on Intel x86_64 / Windows 64-bits
    </p>
</h4>

<p align="center">
    <a href="https://github.com/jczic/ESP32-MPY-Jama/releases/download/v1.2.0/ESP32.MPY-Jama.v1.2.0-macos-universal2.dmg"><img src="/img/btn-download-mac.png" width="250"></a>             
    <a href="https://github.com/jczic/ESP32-MPY-Jama/releases/download/v1.2.0/ESP32.MPY-Jama.v1.2.0-win64.exe"><img src="/img/btn-download-win.png" width="250"></a>
</p>

<h5>
    <p align="center">
        To make it work under Linux :penguin: <a href="#linux">click here</a>!
    </p>
</h5>

---

### :cyclone: &nbsp;Access information dashboards instantly.
<p align="center">
    <img src="/img/screen-networks.png" width="700">
</p>

---

### :cyclone: &nbsp;Connect to a Wi-Fi and create an access point in 2 clicks.
<p align="center">
    <img src="/img/screen-wifi-sta.png" height="280">          
    <img src="/img/screen-wifi-ap.png" height="280">
</p>

---

### :cyclone: &nbsp;Install a new firmware on the flash very easily.
<p align="center">
    <img src="/img/screen-esptool.png" width="700">
</p>

---

### :cyclone: &nbsp;Create, import and run mini-applications with customizable parameters.
<p align="center">
    <img src="/img/screen-jama-funcs.png" width="700"><br />
    You are welcome to share your own Jama Funcs if you want :)<br />
    Use <a href="https://github.com/jczic/ESP32-MPY-Jama/blob/ef2cf1cfbc138dd81a4291fe262d21fccb6dc71a/src/content/Jama%20Funcs%20-%20Template.py">this template</a> to make it!
</p>

---

<a name="build and run"></a>
## :rocket: &nbsp;Build &amp; Run

### Required

  - pyWebView ([Check out on GitHub](https://github.com/r0x0r/pywebview))
    ```console
    python -m pip install pywebview
    ```

  - pySerial ([Check out on GitHub](https://github.com/pyserial/pyserial))
    ```console
    python -m pip install pyserial
    ```

### Run
  
  - Just use python

    ```console
    python SRC/app.py
    ```

---

<a name="linux"></a>

## :penguin: &nbsp;Linux version instructions

This describes how to clone the repository and how to run from source. In the third step you will find instructions how to create a binary from source. All st
eps have been tested on Ubuntu 22.04, but should work with little changes on similar distributions as well.

### Installation

```bash
# clone the repository:
git clone https://github.com/jczic/ESP32-MPY-Jama

# install python modules requirements:
sudo apt install libcairo2-dev libgirepository1.0-dev python3-pyqt5 python3-pyqt5.qtwebengine python3-pyqt5.qtwebchannel libqt5webkit5-dev gir1.2-webkit2-4.0

# initialize python venv:
cd ESP32-MPY-Jama
python3 -m venv venv

. venv/bin/activate

pip3 install wheel setuptools
pip3 install pyserial pywebview[qt] pycairo PyGObject pyinstaller
```

### Running from source

When you executed all steps listed under "Installation" you may run directly from sources by executing these steps:

```bash
cd ESP32-MPY-Jama
. venv/bin/activate
python3 src/app.py
```

### Building executable

Execute the steps listed under "Installation" and then continue like this:

```bash
cd ESP32-MPY-Jama
./create_binary.sh
```

When the script finishes you should end up with a "esp32-mpy-jama" executable in the "dist" subfolder.

---

<a name="author"></a>
## :wink: &nbsp;Author

  **Jean-Christophe Bos** (:fr:)
  - GitHub: *[@jczic](https://github.com/jczic)*
  - Email:  *<jczic.bos@gmail.com>*
  - Profil: *[LinkedIn](https://www.linkedin.com/in/jczic)*
  - Music:  *[SoundCloud](https://soundcloud.com/jczic/sets/electro-pulse)*
            *[Spotify](https://open.spotify.com/album/5fUd57GcAIcdUn9NX3fviG)*
            *[YouTube](https://www.youtube.com/playlist?list=PL9CsGuMbcLaU02VKS7jtR6LaDNpq7MZEq)*
---

<a name="thanks"></a>
## :+1: &nbsp;Special thanks to 

  - **[rdagger](https://github.com/rdagger)** > [www.rototron.info](https://www.rototron.info)
  - **[happenpappen](https://github.com/happenpappen)** > [www.stop.pe](https://stop.pe)

---

<a name="license"></a>
## :eight_pointed_black_star: &nbsp;License

  - Copyright :copyright: 2023 [Jean-Christophe Bos](https://www.linkedin.com/in/jczic).
  - This project is [MIT](https://github.com/jczic/ESP32-MPY-Jama/blob/master/LICENSE.md) licensed.

---

<br />
