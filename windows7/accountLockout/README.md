# Unlock Account

>> Mensagem:
>> A conta referenciada está bloqueada no momento e pode não ser possivel fazer logon.

### Solução 01

- Entrar em modo de segurança
- CMD
```sh
$ net user administrador <senha> active:yes
```

### Solução 02

- Boot
- Reparar (F6)
- CMD
```sh
$ C: ren utilman.exe utilman.bkp
$ copy cmd.exe utilman.exe
$ exit
```
CTRL + U (tela de login) e inserir
```sh
$ net accounts /lockout window:0
```
