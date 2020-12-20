<h3 align="center">LibreRDP</h3>
<p align="center">Freeware patcher that enables concurrent RDP sessions.</p>
<p align="center">
<img src="https://badgen.net/badge/license/MIT/blue" href="#" />
<img src="https://badgen.net/badge/language/C/green" href="#" />
</p>

#### About
Customer versions of Microsoft Windows does not support concurrent RDP connections. If you want multiple people to connect to the same computer, you need to patch the Terminal Server Service (termsrv.dll). There are already existing solutions to this such as [RDPWrap](https://github.com/stascorp/rdpwrap), but the issue with them is that you need to manually update the offsets each time there is a Windows update.

LibreRDP does things a bit differently. Instead of relying on signature scanning or hardcoded offsets, it parses downloaded [debugging symbols](https://en.wikipedia.org/wiki/Debug_symbol) from [Microsoft Public Symbol Server](https://docs.microsoft.com/en-us/windows-hardware/drivers/debugger/microsoft-public-symbols).