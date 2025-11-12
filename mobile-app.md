frida

adb devices

adb shell

adb reboot

uname -m

pip install frida-tools —break-system-packeges

frida-ps -Ua //active process app

frida-ps -Uai //installed app

frida -U -p <pid>

tar xzf <file_name > //unzip_file

adb push frida-server /data/local/tmp

chmod +x frida-server

chmod 755 frida-server


./frida-server & //run frida server


frida-trace -U -i open -p <pid>


frida —codeshare <packeg-name> -U -p <pid>

>pm path <PACKEG_NAME>

adb shell pm path com.example.someapp

adb pull <APP_PATH> <LOCAL_PATH>

pip3 install objection

pip uninstall objection

pip uninstall frida

pip uninstall frida-tools

pip install objection

pip install frida==16.7.19

pip install frida-tools==13.7.1

objection —gadget “<pagkeg_name>” explore


android sslpinning disable

MOBSF>>>>>>>>>>>>>>>>>>>


APKTooL

apktool d ‘<appname>’

apktool b ‘<app_folder_name>’

JADX 




