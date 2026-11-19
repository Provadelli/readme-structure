# Modelo: skill ou biblioteca open source

Base: SEO pro max e Web Quality Engineer (skills do Claude publicadas no GitHub e no skills.sh).

O leitor quer saber, nesta ordem: **o que é, se é seguro baixar, como instalar e como usar.** A seção de segurança é verificável (inventário de arquivos e SHA-256 no `SECURITY.md`).

Substitua tudo entre `<>`.

````md
<div align="center">

![<Nome>: <slogan>](assets/banner.png)

# <Nome>

**<O que é, em uma frase, e o formato (Skill para o Claude, biblioteca npm...).>**

<Segunda frase com o resultado prático.>

![Formato](https://img.shields.io/badge/formato-Claude%20Skill-1d6ad2)
![Conteúdo](https://img.shields.io/badge/conte%C3%BAdo-Markdown%20%2B%201%20imagem-22A068)
![Scripts](https://img.shields.io/badge/scripts%20execut%C3%A1veis-nenhum-22A068)
![Idioma](https://img.shields.io/badge/idioma-pt--BR-1d6ad2)
[![skills.sh](https://skills.sh/b/<usuario>/<repo>)](https://skills.sh/<usuario>/<repo>)

</div>

---

## Sumário

- [O que é](#o-que-é)
- [Para quem serve](#para-quem-serve)
- [Como funciona](#como-funciona)
- [Segurança: por que é tranquilo baixar](#segurança-por-que-é-tranquilo-baixar)
- [Estrutura do projeto](#estrutura-do-projeto)
- [Instalação](#instalação)
- [Como usar no dia a dia](#como-usar-no-dia-a-dia)
- [Princípios](#princípios)
- [Origem](#origem)
- [Perguntas frequentes](#perguntas-frequentes)
- [Licença](#licença)

---

## O que é

<Definição + lista do que a skill cobre, cada item com o termo-chave em negrito.>

## Para quem serve

- <Público e contexto.>

## Como funciona

```text
<diagrama em texto do fluxo ou das fases>
```

## Segurança: por que é tranquilo baixar

> Resumo: <só texto, não executa nada, não pede senha, não acessa a internet>. A política completa, a lista de arquivos e as impressões digitais (SHA-256) estão em [`SECURITY.md`](SECURITY.md).

| Garantia | Detalhe |
|---|---|
| Só texto e uma imagem | <lista exata de tipos de arquivo> |
| Limites escritos na própria skill | <seção "Limites de segurança" do SKILL.md> |
| Integridade verificável | SHA-256 de cada arquivo no `SECURITY.md` |
| Licença aberta | <licença> |

Comandos de conferência para Linux/macOS (`find` + `sha256sum`) e Windows (`Get-ChildItem` + `Get-FileHash`).

## Estrutura do projeto

```text
<repo>/
├── README.md        Este arquivo
├── SKILL.md         Ponto de entrada
├── SECURITY.md      Política, inventário e SHA-256
├── LICENSE
├── .gitattributes   Mantém os arquivos idênticos em qualquer sistema
├── assets/
│   └── banner.png   Imagem de capa (só ilustração)
└── references/
    └── <arquivo>.md <conteúdo>
```

## Instalação

### Pelo skills.sh (recomendado)

```bash
npx skills add <usuario>/<repo>
```

<Explicar que quem roda é a ferramenta oficial `skills`, não a skill; aviso de telemetria e como desligar (`DISABLE_TELEMETRY=1` ou `DO_NOT_TRACK=1`).>

### Claude Code (computador)

```bash
git clone https://github.com/<usuario>/<repo>.git ~/.claude/skills/<repo>
```

### Claude.ai (aplicativo ou web)

1. Baixe em **Code > Download ZIP**.
2. Em **Configurações > Capacidades > Skills**, envie o ZIP.
3. Ative a skill.

## Como usar no dia a dia

| Você pede | O que a skill faz |
|---|---|
| "<pedido natural>" | <comportamento> |

## Princípios

1. <Princípio curto.>

## Origem

<Projetos reais de onde o método saiu, com links, sem dados internos.>

## Perguntas frequentes

**<Pergunta?>**
<Resposta curta.>

## Licença

[MIT](LICENSE). Uso livre, inclusive comercial, mantendo o aviso de licença.
````

## SECURITY.md de uma skill

Seções, nesta ordem: 1. O que a skill é · 2. O que ela NÃO faz (tabela "A skill não... / Como você confere") · 3. Limites que o Claude segue · 4. Instalação pelo skills.sh · 5. Sobre os trechos de código · 6. Inventário e SHA-256 (todos os arquivos menos o próprio `SECURITY.md`) · 7. Como verificar em 2 minutos · 8. Checklist antes de instalar · 9. Relatar um problema · 10. Versões.

O `.gitattributes` com `* -text` garante que as impressões digitais confiram no clone e no ZIP. Atualize a tabela SHA-256 no mesmo commit em que qualquer arquivo mudar.
