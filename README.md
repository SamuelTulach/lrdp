<h3 align="center">LibreRDP</h3>
<p align="center">Freeware patcher that enables concurrent RDP sessions.</p>
<p align="center">
<img src="https://badgen.net/badge/license/MIT/blue" href="#" />
<img src="https://badgen.net/badge/language/C/green" href="#" />
</p>

#### About
Customer versions of Microsoft Windows does not support concurrent RDP connections. If you want multiple people to connect to the same computer, you need to patch the Terminal Server Service (termsrv.dll). There are already existing solutions to this such as [RDPWrap](https://github.com/stascorp/rdpwrap), but the issue with them is that you need to manually update the offsets each time there is a Windows update.

LibreRDP does things a bit differently. Instead of relying on signature scanning or hardcoded offsets, it parses downloaded [debugging symbols](https://en.wikipedia.org/wiki/Debug_symbol) from [Microsoft Public Symbol Server](https://docs.microsoft.com/en-us/windows-hardware/drivers/debugger/microsoft-public-symbols) to patch the file. By using this method, it does not need to be manually updated and is compatible with pretty much any newer 64-bit Windows version.

### Download
You can always download the latest version from [releases section](https://github.com/SamuelTulach/lrdp/releases). Please do not download it from anywhere else since you might encounter malware.

### Issues / Contributing
If you have any issue with this software and you would like to report it, [feel free to use GitHub issues](https://github.com/SamuelTulach/lrdp/issues). Please be as descriptive as possible and attach screenshots. If you want to contribute to this repo, you can make [a pull request](https://github.com/SamuelTulach/lrdp/pulls).