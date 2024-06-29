# powershell-termux
Powershell Installation to termux script

You can copy & paste to termux terminal to install powershell and start powershell everytime you open termux terminal again
```
pkg install proot-distro
proot-distro install debian
echo "proot-distro login debian" >> ~/.bashrc
source ~/.bashrc
apt update
apt install libicu-dev -y
curl -L -o powershell.tar.gz "https://github.com/PowerShell/PowerShell/releases/download/v7.2.6/powershell-7.2.6-linux-arm64.tar.gz"
mkdir powershell
mv powershell.tar.gz powershell/
cd powershell
tar xzvf powershell.tar.gz
echo "./pwsh" >> ~/.bashrc
source ~/.bashrc
```
