# Atividade prática individual - Tópico 4

## Nível realizado
Nível 2 - Intermédio

## Objetivo
Aplicar medidas iniciais de segurança ao serviço publicado no Tópico 3, através da identificação da superfície de ataque e da configuração básica de firewall.

## Ambiente utilizado
VM local com Ubuntu Server no VirtualBox

## Serviço publicado
Apache com site estático publicado no Tópico 3

## Ficheiros criados
- comandos.txt
- superficie-ataque.md
- firewall.md
- validacao.md
- README.md

## Evidências produzidas
- evidencias/portas.png
- evidencias/ufw_Inactive.png
- evidencias/ufw active.png


## Resumo do que foi feito
- Identificação dos serviços ativos e portas abertas.
- Análise da superfície de ataque.
- Verificação do estado inicial do UFW.
- Aplicação de regras para permitir HTTP.
- Validação de que o site continuou acessível após ativar o firewall.

## Resultado obtido
O nível 2 foi concluído com sucesso. O serviço web permaneceu acessível após a aplicação das regras de firewall.

## Dificuldades encontradas
- O UFW estava inicialmente inativo.
- Foi necessário garantir que a porta 80 ficava permitida antes da ativação do firewall.


## Próximos passos
No Tópico 5, devo aprofundar medidas de segurança, como hardening do serviço, revisão de permissões, HTTPS e proteção adicional do sistema.
