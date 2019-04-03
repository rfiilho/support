# Resize

Redimensionar tamanho do HD no Virtualbox.

### Conversão (opcional)
> VBoxManage cloneHD <caminho do disco> <caminho do novo disco> --formatVDI
```sh
$ VBoxManage cloneHD "C:\caminho_do_disco.VMDK" "C:\caminho_do_disco.VDI" --formatVDI
```

### Modificar
> VBoxManage modifyHD <caminho do disco> --resize <tamanho em GB>
```sh
$ VBoxManage modifyHD "C:\caminho_do_disco.VDI" --resize 10000
```
### Gparted
* Desativar SWAP
* Aumentar EXTENDED
* Mover SWAP para fim do disco
* Diminuir EXTENDED
* Aumentar disco principal
