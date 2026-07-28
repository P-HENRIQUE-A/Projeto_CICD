# Projeto CI/CD

Este projeto é uma página estática simples, criada para demonstrar o uso de conceitos básicos de CI/CD, containerização com Docker e publicação em ambientes de deploy.

A aplicação apresenta uma interface simples em HTML e CSS, com estrutura organizada para facilitar testes e implantação.

## Objetivo

O objetivo deste projeto é servir como exemplo prático de:

- criação de uma página web estática;
- uso de Docker para executar a aplicação;
- configuração de pipeline de integração e deploy com GitLab CI;
- organização básica de arquivos para publicação.

## Estrutura do projeto

- `index.html` — página inicial do projeto;
- `templatemo_598_sleeky_pro/` — arquivos HTML, CSS e imagens da interface;
- `Dockerfile` — definição da imagem para servir a aplicação com Apache;
- `docker-compose.yml` — configuração para subir o projeto localmente;
- `.gitlab-ci.yml` — pipeline de validação e deploy.

## Pré-requisitos

Antes de executar o projeto, certifique-se de ter instalado:

- Git
- Docker
- Docker Compose

## Como executar localmente

### Opção 1: abrir diretamente no navegador

Basta abrir o arquivo `index.html` em um navegador.

### Opção 2: executar com Docker

No diretório do projeto, rode:

```bash
docker compose up --build
```

Depois, acesse:

```text
http://localhost:8080
```

## Pipeline CI/CD

O arquivo `.gitlab-ci.yml` configura uma pipeline com duas etapas:

1. `validate` — executa validações básicas no HTML/CSS e testa a página localmente.
2. `deploy` — gera os arquivos públicos para publicação em Pages.

## Como contribuir

1. Clone o repositório:

```bash
git clone <url-do-repositorio>
```

2. Crie uma branch para sua alteração:

```bash
git checkout -b minha-alteracao
```

3. Faça suas alterações, commit e envie para o repositório:

```bash
git add .
git commit -m "Minha alteração"
git push origin minha-branch
```

## Licença

Este projeto é um exemplo didático e pode ser usado e adaptado conforme necessário.
