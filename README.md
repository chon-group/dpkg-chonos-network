# ChonOS Network Manager

|![chonos-network-cover](https://github.com/user-attachments/assets/18c60cc7-949e-4158-bc11-0029d23b38ce)|
|:--:|
|ChonOS Network Manager implements auto management for IEEE 802.3 and IEEE 802.11 network interfaces. So, the designer can easily access the management layer by connecting a network cable from the device directly to a computer or any port in the local area network without worrying about the local Dynamic Host Configuration Protocol server or static IP address. Also, it implements Wi-Fi Direct; thus, the designer can manage it even using a smartphone. Finally, it implements link monitoring and auto-reconnection using Internet Control Message Protocol, which is useful for mobile robots that may eventually leave the range of the wireless network.|

## How to Install?
1) In a terminal run the commands below:

```console
echo "deb [trusted=yes] http://packages.chon.group/ chonos main" | sudo tee /etc/apt/sources.list.d/chonos.list
sudo apt update
sudo apt install chonos-network
```

### DESCRIPTION

TODO

### EXAMPLES

1. Creating a Wireless Access Point named _EmbeddedMAS_ without passowrd:

```sh
sudo chonosWifiConf -m ap -c 1 -e EmbeddedMAS -k NONE
```

2. Join into a Wireless Local Area Network named _MyNetwork_ using _MyPassword_, as password:

```sh
sudo chonosWifiConf -m client -e MyNetwork -k MyPassword
```

## COPYRIGHT
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />The [_Cognitive Hardware on Networks Operating
System (chonOS)_](http://os.chon.group/) and is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>. The licensor cannot revoke these freedoms as long as you follow the license terms:

* __Attribution__ — You must give __appropriate credit__ like below:

Lazarin, N., Pantoja, C., Viterbo, J. (2026). An Operating-System Infrastructure for Embedded BDI-Based Multi-agent Systems. In: Gervasi, O., et al. Computational Science and Its Applications – ICCSA 2026. ICCSA 2026. Lecture Notes in Computer Science, vol 16769. Springer, Cham. [https://doi.org/10.1007/978-3-032-30494-0_37](https://www.researchgate.net/publication/405508586_An_Operating-System_Infrastructure_for_Embedded_BDI-based_Multi-Agent_Systems)


