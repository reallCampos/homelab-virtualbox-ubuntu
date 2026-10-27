# Home Lab de Virtualização: Ubuntu Desktop e Server com OpenSSH

Ambiente de estudo montado no Oracle VirtualBox com duas máquinas virtuais Ubuntu, simulando a administração remota de um servidor Linux.

## Ambiente

| Máquina | Sistema | Função |
|---|---|---|
| linux-ubuntu | Ubuntu Desktop | Cliente (acessa o servidor por SSH) |
| linux_ubuntu_server | Ubuntu Server 26.04.1 LTS | Servidor (OpenSSH Server) |

## O que foi feito

- Criação das máquinas virtuais no VirtualBox
- Instalação do Ubuntu Desktop e do Ubuntu Server
- Instalação e configuração do OpenSSH Server no servidor
- Acesso remoto do Desktop ao Server via SSH
- Navegação básica pelo sistema de arquivos via terminal remoto

## Comandos utilizados

```bash
ip a                          # verificar o endereço IP do servidor
ssh usuario@IP_DO_SERVIDOR    # conectar do Desktop ao Server
lsb_release -a                # confirmar a versão do sistema
ls, cd                        # navegação pelos diretórios
```

## Evidências

### Conexão SSH funcionando
O terminal do Desktop (esquerda) está conectado ao servidor (direita) via SSH.

![SSH funcionando](images/ssh-funcionando.png)

### Versão do sistema (Ubuntu Server)
![Versão do Ubuntu Server](images/lsb-release.png)

> Endereços IP e MAC foram ocultados nas imagens por privacidade.

## Próximos passos

- Criar usuários adicionais e configurar permissões
- Configurar autenticação por chave SSH
- Instalar um serviço web (Apache ou Nginx)
- Documentar a configuração de rede das VMs

## Ferramentas

Oracle VirtualBox, Ubuntu Desktop, Ubuntu Server, OpenSSH
