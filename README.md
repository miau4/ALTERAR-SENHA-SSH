Aqui está uma sugestão de arquivo `README.md` profissional e claro para o seu repositório:

---

# Script de Configuração SSH e Alteração de Senha

Este script automatiza a configuração básica de segurança e acesso do protocolo SSH no seu servidor Linux, além de facilitar a alteração imediata da senha do usuário `root`.

## 📋 Funcionalidades

* **Segurança SSH:** Ativa automaticamente o `PermitRootLogin` e o `PasswordAuthentication`.
* **Compatibilidade Cloud:** Detecta e aplica as mesmas configurações em arquivos de configuração secundários (comuns em provedores como AWS, Oracle e Google Cloud).
* **Gestão de Senha:** Solicita a definição de uma nova senha para o usuário `root` de forma interativa.
* **Aplicação Imediata:** Reinicia o serviço SSH/SSHD automaticamente para que as alterações entrem em vigor sem a necessidade de reboot.

## 🚀 Instalação Rápida

Para instalar ou atualizar o script no seu servidor, utilize o comando abaixo:

```bash
wget -O /usr/bin/alterar-senha "https://raw.githubusercontent.com/miau4/ALTERAR-SENHA-SSH/refs/heads/main/alterar-senha?cache=$(date +%s)" && chmod +x /usr/bin/alterar-senha

```

## 💻 Como Usar

Após a instalação, basta executar o comando abaixo em qualquer diretório do seu terminal:

```bash
alterar-senha

```

O script irá:

1. Configurar o SSH.
2. Solicitar que você digite a nova senha root duas vezes (padrão do sistema).
3. Reiniciar o serviço de SSH automaticamente.

## ⚠️ Requisitos

* **Permissões:** Deve ser executado como `root` ou com privilégios de `sudo`.
* **Sistema:** Compatível com distribuições Linux baseadas em Debian/Ubuntu que utilizam `systemd`.

---

**Desenvolvido por:** Netsimon
