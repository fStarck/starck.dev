# Starck.dev

Este repositório contém o código-fonte do site **Starck.dev**, configurado para ser hospedado na **Hostinger** com deploy automatizado via GitHub Actions.

## 🛠️ Configurações e Deploy

### O que foi feito até agora:

1. **Estrutura inicial do projeto**:
   - Criado um projeto com os arquivos HTML, CSS e JS na pasta local.
   - Adicionado o projeto ao repositório do GitHub.

2. **Hospedagem na Hostinger**:
   - Configurada a conta FTP na Hostinger para o domínio `starck.dev.br`.
   - Diretório remoto: `/domains/starck.dev.br/public_html`.

3. **Deploy automatizado via GitHub Actions**:
   - Configurado um workflow no GitHub Actions para deploy via FTP.
   - Adicionados os secrets ao repositório no GitHub:
     - `FTP_SERVER`: Endereço do servidor FTP.
     - `FTP_USERNAME`: Nome de usuário do FTP.
     - `FTP_PASSWORD`: Senha do FTP.

### Como funciona o Deploy?

- O deploy é acionado automaticamente sempre que há um **push** para a branch `main`.
- O GitHub Actions usa as credenciais FTP configuradas nos secrets para enviar os arquivos para a Hostinger.

### 🗂️ Estrutura do repositório

```plaintext
.
├── .github
│   └── workflows
│       └── deploy.yml  # Arquivo de workflow para deploy automatizado
├── public_html         # Código-fonte do site (HTML, CSS e JS)
├── README.md           # Documentação do projeto
