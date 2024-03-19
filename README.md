# hellogit-8

Depois de algumas tentativas,
descobri que eu já estava na branch master mas não era exibido de forma explicita no meu terminal essa informação.
Através do comando:
                    $ git branch
é que foi possível fazer essa verificação.
Descobri também que eu precisava gerar uma chave pelo terminal do computador e registra-lá no meu githube.
Isso foi feito através dos comandos:
                    $ ssh-keygen
                    (coloque um nome para a sua chave e em seguida de enter)
                    (não é necessário colocar uma senha, aperte enter apenas)
                    $ ls
                    (além do arquivo README.sh que provavelmente você já gerou, exibirá também as chaves geradas, publica e privada)
                    (nome-da-chave  nome-da-chave.pub  README.sh)
                    $ cat nome-da-chave.pub
                    (irá exibir a chave publica que precisa ser registrada no githube, copie essa chave)
                    $ eval "ssh-agent"
                    $ ssh-add nome-da-chave
                    (chave registrada na pasta que você quer subir no githube)
