# Permissões aplicadas

## Ambiente utilizado
VM local 

## Utilizador e grupos
- whoami devolveu o utilizador atual do sistema:

* Utilizador: **vboxuser**

Este comando permite identificar rapidamente a conta atualmente em utilização no sistema Linux.

- O comando `id` apresentou a seguinte informação:

* UID: 1000 (vboxuser)
* GID: 1000 (vboxuser)
* Grupos:

  * adm
  * cdrom
  * sudo
  * dip
  * plugdev
  * users
  * lxd

Este comando permite visualizar o identificador do utilizador, o grupo principal e todos os grupos aos quais o utilizador pertence. A presença no grupo **sudo** indica permissões administrativas, permitindo a execução de comandos com privilégios elevados.

- O comando `groups` apresentou a lista simplificada de grupos do utilizador:

* vboxuser adm cdrom sudo dip plugdev users lxd

Este comando confirma os grupos associados ao utilizador atual, sem apresentar detalhes adicionais como IDs.

## Ficheiros criados
- publico.txt:
- restrito.txt:
- script.sh:
  
## Permissões aplicadas
| Ficheiro     | Permissão | Justificação                                                   |
| ------------ | --------- | -------------------------------------------------------------- |
| publico.txt  | 644       | Pode ser lido por todos mas apenas alterado pelo proprietário. |
| restrito.txt | 640       | Apenas o proprietário pode alterar e o grupo pode consultar.   |
| script.sh    | u+x       | O proprietário pode executar o script.                         |

## Relação com o princípio do menor privilégio
Em vez de dar acesso total (777) a todos os utilizadores, foram atribuídas apenas as permissões necessárias para reduzir riscos de alterações indevidas ou acesso não autorizado.


