# KivyMD_Experiments
a simple repository which includes simple kivyMD programs

### Buildozer Commands to make an APK

+ Go the main working directory where `main.py` is present.
+ Open Terminal and type: `buildozer init`
+ Now `buildozer.spec` should be created into your main working directory
+ Open `buildozer.spec` and you can change the `title`, `package.name` and `package.domain`
+ In the same `buildozer.spec` file, add any extra file extension which are not present in `source.include_exts`
+ Again in the same `buildozer.spec`, uncomment this line `android.logcat_filters = *:S python:D`
+ Then type this command: `sudo apt update`
+ Then type this command: `sudo apt install -y git zip unzip openjdk-8-jdk python3-pip autoconf libtool pkg-config zlib1g-dev libncurses5-dev libncursesw5-dev libtinfo5 cmake libffi-dev libssl-dev`
+ Then type this command: `pip3 install --user --upgrade Cython==0.29.19 virtualenv`  # the --user should be removed if you do this in a venv
+ Now make sure your phone is connected to your ubuntu machine.
+ Now, type this last command: `buildozer android debug deploy run`
