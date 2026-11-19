# Modelo: site / portfólio / landing

Base: Portfólio de Pedro Provadelli (Next.js, bilíngue, WebGL).

README mais curto: sem sumário numerado. O foco é mostrar o site, explicar o que tem de diferente e ensinar a editar o conteúdo.

Substitua tudo entre `<>`.

````md
<div align="center">

<img src="public/<og-image>.jpg" alt="<O que a imagem mostra>" width="720" />

# <Nome do site>

**<Quem é ou o que é, em uma frase.>** <Complemento curto.>

[![Site no ar](https://img.shields.io/badge/site-no%20ar-<cor>?style=for-the-badge&logo=vercel&logoColor=black)](<url>)
[![<Framework>](https://img.shields.io/badge/<Framework>-<versão>-000000?style=for-the-badge&logo=<logo>&logoColor=white)](<site oficial>)

[**Ver o site**](<url>) · [<Rede>](<url>) · [GitHub](<url>)

</div>

---

## Sobre o projeto

<Um parágrafo: framework e modo de renderização, idiomas, hospedagem, identidade visual, cuidado com acessibilidade.>

## Destaques

| | |
|---|---|
| **<Recurso>** | <O que faz e por que é bem feito: desempenho, fallback, acessibilidade.> |

## <Conteúdo exibido> (ex.: Projetos em destaque)

<De onde vem o conteúdo (arquivo fonte única) e a lista com link e uma linha cada.>

- [**<Item>**](<url>) — <descrição curta>.

## Stack

| Camada | Tecnologias |
|---|---|
| Framework | |
| Linguagem | |
| Estilo | |
| Animação | |
| Imagens | |
| Qualidade | |
| Hospedagem | |

## Começando

Requer **<runtime> <versão> ou superior**.

```bash
git clone https://github.com/<usuario>/<repo>.git
cd <repo>
npm install
npm run dev
```

Acesse [http://localhost:<porta>](http://localhost:<porta>).

### Comandos

```bash
npm run dev        # servidor de desenvolvimento
npm run build      # versão de produção
npm run lint       # lint
```

## Estrutura

```text
src/
├── app/           <rotas>
├── components/    <seções>
├── content/       <textos e dados: a fonte única>
└── lib/           <utilitários>
```

## Como <editar o conteúdo principal> (ex.: adicionar um projeto)

1. <Passo com o arquivo exato.>
2. <Comando que regenera o que for derivado.>
3. <O que se atualiza sozinho.>

## Notas

- **<Tema>:** <regra ou pegadinha que quem mexer precisa saber>.

## Contato

**<Nome>** · <papel>

[<Rede>](<url>) · [GitHub](<url>) · [Site](<url>)
````

## Variação: landing de cliente

Para a landing de uma empresa, troque "Projetos em destaque" por **Seções da página** (tabela Seção | Objetivo) e "Contato" por **Cliente e créditos** (quem é o cliente, quem desenvolveu, onde a marca é usada com permissão).
