# Template para Exame de Qualificação

Template **Quarto** para a elaboração do projeto de pesquisa submetido ao
**Exame de Qualificação** do
[Mestrado Profissional em Administração do IFMG - Campus Formiga](https://www.formiga.ifmg.edu.br/mestrado-profissional-em-administracao).

Este repositório disponibiliza apenas os arquivos-fonte do documento. O PDF
final é gerado localmente e não deve ser versionado com **Git/GitHub**.


## Antes de Começar

Este template assume que você já tem instalados:

- **Quarto**
- **TinyTeX**
- **RStudio**, **VS Code** ou editor equivalente
- **R** apenas se for usar código no documento

Se quiser verificar o ambiente, execute:

```bash
quarto check
```


## Como Criar seu Repositório a partir deste Template

Este projeto foi publicado no **GitHub** como um **template**.

Para criar sua cópia:

1. Acesse esta página do repositório no **GitHub**.
2. Clique em `Use this template`.
3. Crie um novo repositório em sua conta com um nome simples, de preferência no
   padrão `qualificacao_nome_sobrenome`, sem acentos e sem espaços, por
   exemplo: `qualificacao_joao_silva`.
4. Mantenha o repositório como **público**, salvo orientação diferente do
   orientador.
5. Copie a URL do repositório criado.
6. Abra o **RStudio**.
7. Clique em `Project > New Project > Version Control > Git`.
8. Na janela de clonagem do **RStudio**, cole a URL do repositório no campo
   `Repository URL`.
9. No campo `Project directory name`, verifique se apareceu o nome do
   repositório criado, por exemplo: `qualificacao_joao_silva`. Se não aparecer,
   escreva manualmente o nome que você escolheu para o repositório.
10. Escolha a pasta em que o projeto será criado no seu computador.
11. Clique em `Create Project` para criar o projeto no seu computador. O
    **RStudio** fará a clonagem do repositório e abrirá o projeto localmente.
12. Renderize o arquivo `src/exame_qualificacao.qmd` para verificar se tudo
    está funcionando.
13. Adicione o orientador como colaborador do repositório no **GitHub**.

A renderização criará o arquivo `src/exame_qualificacao.pdf`. Esse **PDF** não
é versionado no **Git**, pois é gerado automaticamente a partir do arquivo-fonte
do projeto.

Observações:

- ao clonar pelo **RStudio**, o próprio **RStudio** criará automaticamente o
  arquivo de projeto `.Rproj` com o nome do repositório local;
- esse arquivo `.Rproj` é apenas local e não faz parte do conteúdo versionado
  do template.


## Estrutura do Projeto

Os principais arquivos são:

- `src/exame_qualificacao.qmd`: arquivo principal do projeto;
- `src/pre_textuais.tex`: camada LaTeX reutilizável dos elementos pré-textuais;
- `src/referencias.bib`: arquivo da bibliografia;
- `src/associacao-brasileira-de-normas-tecnicas-ipea.csl`: estilo de citações e referências.

Na maior parte do tempo, você precisará editar apenas
`src/exame_qualificacao.qmd`.

Não altere `src/pre_textuais.tex`, salvo orientação expressa do orientador.


## O que Editar Primeiro

Abra `src/exame_qualificacao.qmd` e revise primeiro o bloco
`DADOS EDITÁVEIS DO EXAME`, no topo do arquivo.

Revise principalmente:

- nome do discente;
- título e subtítulo, se houver;
- cidade, estado e ano;
- orientador;
- coorientador, se houver;
- linha de pesquisa;
- texto de apresentação na folha de rosto.

Regra importante:

- no bloco de dados editáveis, altere apenas o texto entre chaves `{}` e não
  mude o nome dos comandos.

Regras práticas:

- se não houver subtítulo, deixe `\\SubtituloExameQualificacao{}` vazio;
- se não houver coorientador, deixe `\\CoorientadorExameQualificacao{}` vazio;
- na maior parte dos casos, não é necessário editar `src/pre_textuais.tex`;
- evite usar os caracteres `%`, `&`, `#` e `_` nos campos editáveis do topo; se
  isso for indispensável, peça orientação ao orientador;
- as listas de figuras e tabelas são opcionais e só devem ser ativadas se
  realmente houver figuras ou tabelas no texto.


## Estrutura Lógica do Documento

A estrutura textual atual do template foi reorganizada para ficar mais aderente
ao projeto de pesquisa segundo a **ABNT** e ao processo de qualificação do
**PPGA**.

Sequência principal:

1. Introdução
2. Revisão da Literatura
3. Metodologia
4. Resultados esperados e contribuições
5. Cronograma
6. Considerações finais do projeto
7. Referências

Na estrutura atual do template, a seção **Introdução** contém as seguintes
subseções:

- problema de pesquisa;
- hipóteses ou pressupostos, se couber;
- objetivo geral;
- objetivos específicos;
- justificativa.

Importante:

- os objetivos agora ficam dentro da **Introdução**, e não mais como capítulo
  independente;
- a seção de cronograma foi simplificada para uma tabela em Markdown, sem
  necessidade de editar código em **R**;
- os elementos pré-textuais passaram a ser controlados internamente pelo
  template, de modo que o orientando normalmente só precisa editar os campos do
  topo do arquivo principal.


## Como Escrever o Texto

No arquivo `src/exame_qualificacao.qmd`, o aluno deve:

- escrever o texto principal nas seções já criadas;
- apagar subseções que não se aplicarem ao projeto, como hipóteses ou aspectos
  éticos, quando for o caso;
- substituir a tabela de cronograma pelas etapas reais da pesquisa;
- incluir as referências bibliográficas em `src/referencias.bib`.


## Gerando o PDF

No **RStudio**, clique em `Render`, ou use no terminal:

```bash
quarto render src/exame_qualificacao.qmd
```

O PDF será gerado na pasta `src/` e não deve ser enviado ao repositório.


## Dicas de Uso

- citações: `@sobrenome2023`
- seções: `#`, `##`, `###`
- imagens: `![Legenda](caminho/para/imagem.png)`
- referência cruzada: `{#sec-id}` e `@sec-id`


## Suporte

- Documentação do Quarto: <https://quarto.org/docs/guide/>
- Orientações do orientador
- Abertura de issue neste repositório, se necessário
