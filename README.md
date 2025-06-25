# VSCode_Test_MIC:with_GPT

- Debian ALSA [![alt text][1]](https://wiki.debian.org/ALSA)
- Debian which sound system is active [![alt text][1]]()
- Is there a reason for an App to use the pipewire API over ALSA? [![alt text][1]](https://stackoverflow.com/questions/78008373/is-there-a-reason-for-an-app-to-use-the-pipewire-api-over-alsa)
- Quickstart: Install the Speech SDK - Linux/Debian requirement [![alt text][1]](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/quickstarts/setup-platform?tabs=linux%2Cdebian%2Cdotnetcli%2Cjre%2Cmaven%2Cnodejs%2Cmac%2Cpypi&pivots=programming-language-csharp#tabpanel_1_linux)
- One of the following commands might give you what you are after [![alt text][1]](https://superuser.com/questions/47146/how-can-i-find-out-what-programs-are-using-sound-in-linux)
- YouTube Vid- Release Party v1.87 | VS Code Speech and Copilot Extensibility [![alt text][1]](https://www.youtube.com/watch?v=7PtNKleyHNk)

## Start of project

<!-- -->
```bash
> date
Wed Jun 25 06:35:25 PM CEST 2025
```

## Install on Debian

- OS release
<!-- -->
```bash
    > Cat /etc/os-release 
    PRETTY_NAME="Debian GNU/Linux 12 (bookworm)"
    NAME="Debian GNU/Linux"
    VERSION_ID="12"
    VERSION="12 (bookworm)"
    VERSION_CODENAME=bookworm
    ID=debian
    HOME_URL="https://www.debian.org/"
    SUPPORT_URL="https://www.debian.org/support"
    BUG_REPORT_URL="https://bugs.debian.org/"
```
<!-- -->
- OS point release
<!-- -->
```bash
> cat /etc/debian_version
12.11
```

- MS VS Code Version - from the MS Vscode help menu
<!-- -->
```text
Version: 1.101.1
Commit: 18e3a1ec544e6907be1e944a94c496e302073435
Date: 2025-06-18T13:35:12.605Z
Electron: 35.5.1
ElectronBuildId: 11727614
Chromium: 134.0.6998.205
Node.js: 22.15.1
V8: 13.4.114.21-electron.0
OS: Linux x64 6.1.0-37-amd64
```
<!-- -->
## Setup/Install nectary OS/Debian packages [![alt text][1]](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/quickstarts/setup-platform?tabs=linux%2Cdebian%2Cdotnetcli%2Cjre%2Cmaven%2Cnodejs%2Cmac%2Cpypi&pivots=programming-language-csharp#tabpanel_1_linux)
<!-- -->
```bash
sudo apt-get update
sudo apt-get install build-essential ca-certificates libasound2-dev libssl-dev wget
```

## Check/install MS Vscode extension

>[!TIP]
><!-- -->
>```bash
Extensions Management
  --extensions-dir <dir>              Set the root path for extensions.
  --list-extensions                   List the installed extensions.
  --show-versions                     Show versions of installed extensions,
                                      when using --list-extensions.
  --category <categ ory>               Filters installed extensions by provided
                                      category, when using --list-extensions.
  --install-extension <ext-id | path> Installs or updates an extension. The
                                      argument is either an extension id or a
                                      path to a VSIX. The identifier of an
                                      extension is '${publisher}.${name}'. Use
                                      '--force' argument to update to latest
                                      version. To install a specific version
                                      provide '@${version}'. For example:
                                      'vscode.csharp@1.2.3'.
  --pre-release                       Installs the pre-release version of the
                                      extension, when using
                                      --install-extension
  --uninstall-extension <ext-id>      Uninstalls an extension.
  --update-extensions                 Update the installed extensions.
  --enable-proposed-api <ext-id>      Enables proposed API features for
                                      extensions. Can receive one or more
                                      extension IDs to enable individually.

>```
<!-- -->

- check is already installed
<!-- -->
```bash
> code --list-extensions |grep speech
ms-vscode.vscode-speech
ms-vscode.vscode-speech-language-pack-de-de
```
<!-- -->
- install via command line/bash



> [!NOTE]
> Supported Languages

The VS Code Speech extension supports 26 languages in total. You can configure the setting accessibility.voice.speechLanguage to the desired language for speech recognition and synthesis. This may require additional extensions to be installed for the language support.
<!-- -->
<!-- Link sign - Don't Found a better way :-( - You know a better method? - send me a email,please -->
[1]: img/link_symbol.svg