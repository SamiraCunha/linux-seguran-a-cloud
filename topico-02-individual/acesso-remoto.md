# Acesso remoto por SSH

## Estado do serviço SSH

Ao verificar o estado do serviço com o comando `systemctl status ssh`, foi apresentada a mensagem “Unit ssh.service could not be found”, indicando que o serviço SSH não estava disponível no ambiente inicial.

Após isso, foi realizada a instalação do serviço com `sudo apt install openssh-server` e o serviço foi ativado com `sudo systemctl enable ssh` e `sudo systemctl start ssh`, passando a ficar disponível no sistema.

---

## Endereço identificado
10.0.2.15

---

## Comando de ligação

Exemplo de ligação ao servidor via SSH:

```bash id="2kq8vn"
ssh utilizador@endereco_ip
```

---

## Resultado obtido

Após a instalação e ativação do serviço, o SSH passou a estar funcional, permitindo ligações remotas ao sistema (caso o serviço esteja ativo e configurado corretamente).

---

## Limitações encontradas

O serviço SSH não estava disponível inicialmente no ambiente utilizado, sendo necessário proceder à sua instalação e configuração manual para permitir o acesso remoto.
