# ChonOS Network Manager

|![chonos-firmware](https://github.com/chon-group/dpkg-chonos-firmwaremng/assets/32855001/f4f43941-6fdb-4b58-9791-66f480c0d449)|
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
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />The Chonos Network Manager is part of the [_Cognitive Hardware on Networks Operating
System (chonOS)_](http://os.chon.group/) and is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>. The licensor cannot revoke these freedoms as long as you follow the license terms:

* __Attribution__ — You must give __appropriate credit__ like below:

LAZARIN, Nilson Mori; PANTOJA, Carlos Eduardo; VITERBO, José. Towards a Toolkit for Teaching AI Supported by Robotic-agents: Proposal and First Impressions. In: WORKSHOP SOBRE EDUCAÇÃO EM COMPUTAÇÃO (WEI), 31. , 2023, João Pessoa/PB. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2023 . p. 20-29. ISSN 2595-6175. DOI: https://doi.org/10.5753/wei.2023.229753.


<details>
<summary> Bibtex citation format</summary>

```
@inproceedings{chonOS,
 author = {Nilson Lazarin and Carlos Pantoja and José Viterbo},
 title = { Towards a Toolkit for Teaching AI Supported by Robotic-agents: Proposal and First Impressions},
 booktitle = {Anais do XXXI Workshop sobre Educação em Computação},
 location = {João Pessoa/PB},
 year = {2023},
 issn = {2595-6175},
 pages = {20--29},
 publisher = {SBC},
 address = {Porto Alegre, RS, Brasil},
 doi = {10.5753/wei.2023.229753},
 url = {https://sol.sbc.org.br/index.php/wei/article/view/24887}
}

```
</details>
