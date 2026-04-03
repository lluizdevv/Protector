# 🔐 Protector - Gerenciador de Senhas

O **Protector** é um sistema de gerenciamento de senhas desenvolvido em Python, com foco em **segurança, organização e conscientização digital**.

O projeto foi criado no contexto acadêmico da UFRPE com o objetivo de oferecer uma ferramenta capaz de armazenar senhas de forma segura, além de auxiliar o usuário na criação e análise de credenciais fortes.



## 📌 Motivação

Com o crescimento dos ataques cibernéticos e vazamentos de dados, proteger informações pessoais se tornou essencial.

Muitos usuários ainda utilizam senhas fracas ou repetidas, o que aumenta significativamente os riscos de invasão. O **Protector** surge como uma solução para:

- Armazenar senhas com segurança  
- Incentivar boas práticas de segurança digital  
- Detectar possíveis vazamentos de credenciais  
- Alertar o usuário sobre riscos  



## 🎯 Objetivo

Desenvolver um sistema que permita:

- Gerenciamento seguro de senhas  
- Autenticação de usuários  
- Criação de múltiplos perfis  
- Monitoramento de segurança  
- Educação do usuário sobre boas práticas  



## 🚀 Funcionalidades

### 🔐 Autenticação e Segurança
- Cadastro e login de usuários  
- Bloqueio de conta após 3 tentativas inválidas  
- Notificação por e-mail em caso de bloqueio  



### 👤 Gestão de Usuários e Perfis
- CRUD completo de usuários  
- Criação de múltiplos perfis por usuário  
- Seleção de perfil para uso do sistema  



### 🔑 Gerenciamento de Senhas
- Cadastro de novas senhas  
- Atualização de senhas existentes  
- Exclusão de senhas  
- Listagem e visualização de dados  



### ⚙️ Ferramentas de Segurança
- Gerador de senhas fortes  
- Avaliador de força de senha  
- Verificador de senhas vazadas (API externa)  



### 💾 Persistência de Dados
- Armazenamento em arquivo JSON  
- Estrutura organizada e modular  



## 🛠️ Tecnologias Utilizadas

- **Python**
- **Visual Studio Code**

### 📚 Bibliotecas

- `requests` → consumo de APIs  
- `hashlib` → criptografia de dados  
- `re` → validações com regex  
- `os` → manipulação de arquivos  
- `time` → controle de execução  
- `string` → manipulação de textos  
- `secrets` → geração segura de dados  
- `smtplib` → envio de e-mails  
- `json` → persistência de dados  



## 📂 Estrutura do Projeto

```
protector/
│
├── main.py                # Ponto de entrada da aplicação
├── requirements.txt       # Dependências do projeto
│
├── src/
│   │
│   ├── servicos/
│   │   ├── sistema_gerenciador.py   # Lógica central do sistema
│   │   └── email.py                 # Serviço de envio de e-mails
│   │
│   ├── usuario/
│   │   ├── usuario.py               # Classe de usuário
│   │   └── perfil.py                # Classe de perfil
│   │
│   ├── utilitario/
│   │   ├── validadores.py           # Validações de dados
│   │   ├── limpeza.py               # Limpeza do terminal
│   │   └── geradores.py             # Gerador de senhas
│   │
│   └── menu/
│       └── menus.py                 # Gerenciamento dos menus
│
├── dados.json            # Persistência de dados
│
└── README.md             # Documentação
```



## ⚙️ Como Executar o Projeto

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/seu-usuario/protector.git
cd protector
```



### 2️⃣ Instalar dependências

```bash
pip install -r requirements.txt
```



### 3️⃣ Executar o sistema

```bash
python main.py
```



## 🔄 Fluxo do Sistema

### 🧾 Cadastro
- Usuário informa dados (nome, email, login, senha)
- Sistema valida:
  - Campos obrigatórios  
  - Email válido  
  - Usuário não existente  
- Após sucesso → acesso ao menu de perfis  


### 🔑 Login
- Usuário informa credenciais  
- Sistema verifica:
  - Se correto → acesso liberado  
  - Se incorreto → incrementa tentativas  
  - Após 3 erros → bloqueio + envio de e-mail  



### 👤 Perfis
- Criar novo perfil  
- Selecionar perfil existente  
- Acessar funcionalidades do sistema  



### 📌 Menu Principal
- Gerenciar senhas  
- Gerar senha segura  
- Visualizar dados  
- Trocar perfil  



## 🔐 Segurança Implementada

- Criptografia de dados sensíveis  
- Bloqueio por tentativas de login  
- Verificação de senhas vazadas  
- Notificação por e-mail  
- Persistência segura em JSON  



## 🧪 Testes

- Testes realizados manualmente  
- Validação de fluxos principais  
- Testes de tratamento de erros  



## 💡 Diferenciais do Projeto

- Integração com API para verificar vazamento de senhas  
- Sistema de notificação por e-mail  
- Estrutura modular bem organizada  
- Foco em segurança real do usuário  


## 🔮 Melhorias Futuras

- Interface gráfica (GUI)  
- Testes automatizados  
- Ocultação de senhas na tela  
- Melhorias de usabilidade  



## 👨‍💻 Autores

- Danielly Nunes
- Luiz Vinicius     

Universidade Federal Rural de Pernambuco - UFRPE  



## 📚 Licença

Este projeto foi desenvolvido para fins acadêmicos.
