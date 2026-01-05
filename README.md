# Template para Exame de Qualificação

Template **Quarto** para elaboração do documento necessário para o **Exame de Qualificação**
do [**Mestrado Profissional em Administração do IFMG – Campus Formiga**](https://www.formiga.ifmg.edu.br/mestrado)

Este repositório disponibiliza **apenas os arquivos-fonte** do documento.
O arquivo PDF final é **gerado localmente** pelo orientando e 
**não deve ser versionado com Git/GitHub**.


## Caminho rápido 

1. Clique em **Use this template**
2. Crie um novo repositório em sua conta
3. Clone o repositório no seu computador
4. Abra o projeto no RStudio (ou editor equivalente)
5. Gere o PDF: Clicando em Render ou via terminal com:
   
```bash
quarto render src/exame_qualificacao.qmd
```

As seções seguintes detalham a estrutura e o uso do template.


# Estrutura do Template

A estrutura básica do template é a seguinte:

``` 
.
├── src/
│   ├── exame_qualificacao.qmd
│   ├── pre_textuais.tex
│   ├── referencias.bib
│   └── associacao-brasileira-de-normas-tecnicas-ipea.csl
├── README.md
└── .gitignore
```

Importante: não renomeie nem mova os arquivos da pasta `src/`.

# Descrição dos arquivos

- `src/exame_qualificacao.qmd`

Arquivo principal em formato Quarto, onde o texto do Exame de Qualificação
deve ser redigido.

- `src/pre_textuais.tex`

Arquivo LaTeX para personalização da capa, resumo, palavras-chave e demais
elementos pré-textuais.

- `src/referencias.bib`

Arquivo para gerenciamento das referências bibliográficas.

- `src/associacao-brasileira-de-normas-tecnicas-ipea.csl`

Arquivo de estilo para formatação das citações e referências 
conforme ABNT.



# Pré-requisitos

Para utilizar este template, é necessário ter instalado:

-	Quarto (versão mais recente)
-	Um editor de texto:
-	RStudio, VS Code ou Positron
-	TinyTeX
-	R ou Python (apenas se o documento contiver códigos)

Recomenda-se verificar a instalação com:

```
quarto check
```


# Usando o template

## Criando o repositório no GitHub:

1.	Clique em `Use this template`
2.	Selecione `Create a new repository`
3.	Escolha um nome (ex.: exame_qualificacao_seunome)
4.	Crie o repositório


## Abrindo o projeto no RStudio:

1.	`File` → `New Project` → `Version Control` → `Git`
2.	Cole a URL do seu repositório
3.	Escolha o diretório local
4.	Clique em `Create Project`



## Editando o documento
	
- Texto principal: `src/exame_qualificacao.qmd`

- Capa e pré-textuais: `src/pre_textuais.tex`

- Referências bibliográficas: `src/referencias.bib`



# Gerando o PDF

Clique em Render no RStudio ou execute no terminal:

```
quarto render src/exame_qualificacao.qmd
```

O PDF é gerado localmente e não deve ser adicionado ao 
repositório Git.



# Compartilhando com o orientador

1.	No GitHub, acesse **Settings → Collaborators**
2.	Clique em **Add people**
3.	Informe o usuário ou **e-mail** do orientador
4.	Conceda permissão Write ou Maintain



# Estrutura do documento gerado

- Capa institucional do IFMG
- Resumo e palavras-chave
- Sumário automático
- Introdução
- Justificativa
- Objetivos (geral e específicos)
- Revisão de Literatura
- Metodologia
- Resultados Esperados
- Cronograma
- Referências
- Apêndices/Anexos (opcional)


# Dicas de uso:

- Citações: `@sobrenome2023`
- Seções: #, ##, etc.
- Imagens externas: `![Legenda](caminho/para/imagem.png)`
- Referência cruzada: `{#sec-id}` e `@sec-id`



# Suporte

- Documentação do Quarto: https://quarto.org/docs/guide/
- Contato com o orientador
- Abertura de issue neste repositório


