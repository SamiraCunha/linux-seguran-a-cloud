# Superfície de ataque

## Serviço web identificado
O serviço web usado no Tópico 3 é o Apache.

## Serviços ativos observados
- sshd
- apache2
- systemd-resolve
- chronyd
- systemd-networkd

## Portas abertas ou em escuta
| Porta | Protocolo | Serviço | Necessidade |
|------|-----------|---------|-------------|
| 22 | TCP | SSH (sshd) | Necessária apenas se for preciso acesso remoto por SSH |
| 80 | TCP | HTTP (apache2) | Necessária para publicar o site web |
| 53 | TCP/UDP | DNS local (systemd-resolve) | Necessária para resolução de nomes no sistema |
| 323 | UDP | chronyd | Necessária para sincronização de tempo |

## Portas necessárias para o serviço publicado
A porta 80 é necessária porque o site do Tópico 3 é acedido por HTTP no Apache.  
A porta 22 só é necessária se eu precisar de administrar a VM por SSH.  
As restantes portas observadas são serviços internos do sistema e não fazem parte da publicação do site.

## Riscos iniciais
- O SSH exposto na porta 22 pode ser alvo de tentativas de login se a VM estiver acessível na rede.
- O Apache na porta 80 comunica em HTTP, sem encriptação.
- Qualquer serviço desnecessário em escuta aumenta a superfície de ataque e deve ser revisto.
