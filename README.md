# Desafio-DIO

Repositório criado para consolidar os conhecimentos adquiridos no laboratório prático da DIO sobre provisionamento e conectividade na AWS.

## 📋 Descrição do Projeto
Este projeto documenta o provisionamento de servidores virtuais (EC2) utilizando diferentes sistemas operacionais (Linux e Windows), configurando camadas de segurança e métodos de acesso remoto.

## 🛠️ Etapas do Laboratório

### 1. Provisionamento de Instâncias
Foram criadas **3 instâncias EC2** com as seguintes nomenclaturas:
* **Servidor 1 e 2:** Ambiente Linux.
* **Servidor 3:** Ambiente Windows Server.

### 2. Gestão de Acesso (Key Pairs)
* Criação e download de pares de chaves (.pem/.ppk) para autenticação segura.
* Diferenciação entre chaves para acesso via terminal (SSH) e chaves para descriptografia de senha de administrador (RDP).

### 3. Configuração de Rede e Segurança (Security Groups)
Configuração de regras de entrada (*Inbound Rules*) para permitir a comunicação:
* **Porta 22 (SSH):** Liberada para conexão remota aos servidores Linux.
* **Porta 3389 (RDP):** Liberada para acesso via área de trabalho remota aos servidores Windows.

### 4. Conectividade
A validação do acesso foi realizada com sucesso através das ferramentas:
* **MobaXterm:** Utilizado para acesso SSH às instâncias Linux.
* **RDP Client:** Acesso ao Windows via Console AWS, utilizando a chave privada para obter a senha de administrador.

## 🧠 Insights e Aprendizados
* **Segurança Stateful:** Entendimento de como os Security Groups lembram o estado da conexão, facilitando a configuração de regras de retorno.
* **Isolamento:** A importância de nomear e taguear instâncias para organização em ambientes Cloud.
* **Segregação de Portas:** A boa prática de não abrir todas as portas (0.0.0.0/0) e sim focar nos protocolos necessários para cada serviço.
  
---
Documentação desenvolvida como parte do desafio prático da DIO.
