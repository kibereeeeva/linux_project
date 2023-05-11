# linux_project
## Постановка задачи: необходимо подключиться по SSH протоколу к компьютеру, далее надо выяснить, есть ли на нем jupyter notebook, и, если есть, выяснить его порт и подключиться к нему.
##  Исполнение
Для установки SSH-соединения, необходимо знать адрес SSH-сервера и иметь SSH-клиент в shell. SSH-клиент это программа для доступа к удаленной машине. Она позволяет установить зашифрованную защищенную коммуникацию между двумя хостами даже через небезопасную сеть. Ниже представлены шаги, позволяющие выполнить поставленную задачу.
### Шаги
1. Проверить, есть ли SSH-клиент: `man ssh`
`SSH(1)                    BSD General Commands Manual                   SSH(1)

NAME
     ssh — OpenSSH remote login client

SYNOPSIS
     ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface] [-b bind_address]
         [-c cipher_spec] [-D [bind_address:]port] [-E log_file]
         [-e escape_char] [-F configfile] [-I pkcs11] [-i identity_file]
         [-J destination] [-L address] [-l login_name] [-m mac_spec]
         [-O ctl_cmd] [-o option] [-p port] [-Q query_option] [-R address]
         [-S ctl_path] [-W host:port] [-w local_tun[:remote_tun]] destination
         [command [argument ...]]

DESCRIPTION
     ssh (SSH client) is a program for logging into a remote machine and for
     executing commands on a remote machine.  It is intended to provide secure
     encrypted communications between two untrusted hosts over an insecure
     network.  X11 connections, arbitrary TCP ports and UNIX-domain sockets
     can also be forwarded over the secure channel.

     ssh connects and logs into the specified destination, which may be speci‐
     fied as either [user@]hostname or a URI of the form`

