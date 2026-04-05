# Template para Exame de Qualificação

Template **Quarto** para a elaboração dos projetos de pesquisa de meus 
orientandos que serão submetidos ao **Exame de Qualificação** do 
[Mestrado Profissional em Administração do IFMG - Campus Formiga](https://www.formiga.ifmg.edu.br/mestrado-profissional-em-administracao).



## Antes de começar

1. Para usar este template, é necessário que você tenha instalados:

- **Quarto**
- **TinyTeX**
- **RStudio** (ou outro IDE de sua preferência)
- **R** (apenas se for usar código no documento)

Se quiser verificar o ambiente do sistema Quarto, digite no terminal
Git Bash ou Windows PowerShell: 

```bash
quarto check
```

2. **Recomendo fortemente** que você **atualize** as versões dos 
seguintes softwares antes de começar a usar o template:

- **RStudio**
- **Quarto**

e também a versão de R e dos pacotes usados, caso seja necessário.



## Como criar seu repositório a partir deste template e cloná-lo?

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



## Uso do README.md após criar sua cópia do template

Após criar seu repositório a partir deste template e cloná-lo para seu
computador, recomenda-se adaptar o arquivo `README.md` para que ele passe a
documentar a evolução do seu projeto de pesquisa.

Inicialmente, este arquivo funciona como um guia de uso do template. Com o
avanço do trabalho, porém, ele pode ser reescrito gradualmente para registrar
informações específicas do projeto, como título provisório, objetivo geral,
decisões de estrutura, pendências, reuniões de orientação e principais
alterações realizadas.

Assim, o `README.md` deixa de ser apenas uma instrução inicial de uso do
template e passa a funcionar também como um registro da evolução da
escrita do projeto.



## Estrutura do projeto

Os arquivos mais importantes do template estão na pasta `src/`, que contém
os arquivos-fonte usados para gerar o PDF do projeto.

Os principais arquivos dessa pasta são:

- `src/exame_qualificacao.qmd`: arquivo principal do projeto e principal
  arquivo a ser editado;
- `src/pre_textuais.tex`: arquivo auxiliar com a configuração dos elementos
  pré-textuais;
- `src/referencias.bib`: arquivo da bibliografia;
- `src/associacao-brasileira-de-normas-tecnicas-ipea.csl`: arquivo de estilo
  das citações e referências.

O repositório também contém o arquivo `.gitignore`, que controla quais
arquivos devem ser ignorados pelo Git. Em geral, ele evita o versionamento
de arquivos temporários, arquivos de sistema, arquivos auxiliares do RStudio
e arquivos de saída gerados automaticamente.

Salvo em raras situações, você deverá editar apenas o arquivo
`src/exame_qualificacao.qmd` e atualizar o arquivo `src/referencias.bib`
quando necessário.

Não altere `src/pre_textuais.tex` nem o arquivo `.gitignore`, salvo
orientação expressa do orientador.



## O que editar primeiro?

Abra `src/exame_qualificacao.qmd` e revise primeiro o bloco
`DADOS EDITÁVEIS DO EXAME`, no topo do arquivo.

Inicialmente, edite os seguintes campos:

- nome do discente;
- título e subtítulo se houver (use um título provisório, caso não tenha nenhum);
- cidade, estado e ano;
- orientador;
- coorientador, se houver;
- linha de pesquisa;
- palavras-chave;
- texto de apresentação na folha de rosto.

**Regra importante:**

- no bloco de dados editáveis, altere apenas o texto entre chaves `{}` e não
  mude o nome dos comandos.

**Regras práticas:**

- se não houver subtítulo, deixe `\\SubtituloExameQualificacao{}` vazio;
- se não houver coorientador, deixe `\\CoorientadorExameQualificacao{}` vazio;
- na maior parte dos casos, não é necessário editar `src/pre_textuais.tex`;
- evite usar os caracteres `%`, `&`, `#` e `_` nos campos editáveis do topo; se
  isso for indispensável, peça orientação ao orientador;
- as listas de figuras e tabelas são opcionais e só devem ser ativadas se
  realmente houver figuras ou tabelas no texto.



## Estrutura Lógica do Documento

A estrutura lógica do template foi reorganizada para ficar mais aderente
ao formato de projeto de pesquisa, às normas da **ABNT** e ao processo de
qualificação do **PPGA/IFMG**.

A estrutura principal do documento é a seguinte:

1. Resumo com palavras-chave
2. Introdução
   - problema de pesquisa
   - objetivo geral
   - objetivos específicos
   - justificativa
   - hipóteses (subseção opcional, **insira** quando cabível)
3. Revisão da Literatura
   - lacuna de pesquisa
4. Metodologia
5. Resultados esperados
   - produto bibliográfico
   - produto técnico/tecnológico
   - impactos esperados
6. Cronograma
7. Referências



## Como escrever o texto?

No arquivo `src/exame_qualificacao.qmd`, você deve:

- incluir as referências bibliográficas em `src/referencias.bib`;
- escrever o texto principal nas seções já criadas;
- editar a tabela de cronograma, inserindo as etapas reais planejadas.

Embora essa não seja a ordem final de apresentação do texto no documento,
recomenda-se a seguinte ordem de escrita, por facilitar a evolução gradual
da redação do projeto:

1. Revisão da Literatura
   1.1 Lacuna de Pesquisa
2. Problema de pesquisa
3. Hipóteses (inserir quando cabível)
4. Objetivo geral e objetivos específicos
5. Justificativa
6. Metodologia
7. Resultados esperados
   7.1 Produto bibliográfico
   7.2 Produto técnico/tecnológico
   7.3 Impactos esperados
8. Cronograma
9. Introdução (texto inicial com uma visão geral do projeto)
10. Resumo e palavras-chave
11. Revisão do título e subtítulo (se houver) do projeto



## Gerando o PDF

No **RStudio**, clique em `Render`, ou use no terminal:

```bash
quarto render src/exame_qualificacao.qmd
```

O PDF será gerado na pasta `src/`.



## Referências cruzadas

O sistema **Quarto** permite criar referências cruzadas internas para seções,
equações, figuras e tabelas. Para isso, cada elemento deve receber um
identificador e, depois, esse identificador pode ser citado no texto.

### Seções

Para criar uma referência cruzada para uma seção, atribua um identificador
ao título da seção:

```markdown
## Metodologia {#sec-metodologia}
```

Depois, faça a referência no texto com:

```markdown
Veja a @sec-metodologia.
```

### Equações

Para criar uma referência cruzada para uma equação em bloco, atribua um 
identificador ao bloco da equação. 

Recomenda-se usar identificadores iniciados por `eq-`.

Exemplo:

```markdown
$$
y = \beta_0 + \beta_1 x + u
$$ {#eq-regressao-linear}
```

Depois, faça a referência no texto com:

```markdown
Veja a @eq-regressao-linear.
```

Ao renderizar o documento, o **Quarto** numerará a equação
automaticamente e substituirá a referência pelo número correspondente.

### Figuras inseridas diretamente no texto

Para inserir uma figura diretamente no arquivo `.qmd` e permitir sua
referência no texto, atribua um identificador à figura. É necessário usar
identificadores iniciados por `fig-`.

Exemplo:

```markdown
![Fluxo do processo de pesquisa](figuras/processo.png){#fig-processo}
```

Depois, faça a referência no texto com:

```markdown
Como mostra a @fig-processo, o estudo segue várias etapas.
```

### Figuras geradas por código

Quando a figura é produzida em um bloco de código, o identificador deve
ser definido nas opções da célula de código. Nesse caso, também é necessário 
usar identificadores iniciados por `fig-`.

Exemplo com R:

```{r}
#| label: fig-histograma
#| fig-cap: "Histograma da variável de interesse"

hist(x)
```


Depois, faça a referência no texto com:

```markdown
Veja a @fig-histograma.
```

### Tabelas geradas por código

Para tabelas produzidas programaticamente, o identificador também deve
ser definido nas opções do chunk. É necessário usar identificadores
iniciados por `tbl-`.

Exemplo com R:

```{r}
#| label: tbl-resumo
#| tbl-cap: "Estatísticas descritivas da amostra"

knitr::kable(head(mtcars))
```


Depois, faça a referência no texto com:

```markdown
Os principais resultados descritivos estão na @tbl-resumo.
```

### Convenção recomendada para identificadores

Para as referências cuzuzadas funcionarem é necessário seguir uma 
convenção de nomenclatura para os identificadores dos elementos 
referenciado:

- seções: `sec-...`
- equações: `eq-...`
- figuras: `fig-...`
- tabelas: `tbl-...`

Exemplos:

- `sec-metodologia`
- `eq-capm`
- `fig-fluxograma`
- `tbl-estatisticas-descritivas`


### Recomendações práticas

- use identificadores curtos, informativos e sem acentos;
- **não use** espaços e caracteres especiais nos identificadores;
- **não repita** o mesmo identificador em elementos diferentes;
- ao criar figuras e tabelas por código, informe também uma legenda
  (`fig-cap` ou `tbl-cap`);
- após inserir novos rótulos, renderize novamente o documento para verificar
  se as referências cruzadas foram resolvidas corretamente.



## Suporte

- Documentação do sistema Quarto: <https://quarto.org/docs/guide/>
- Instruções do orientador
- Abertura de issue neste repositório, se necessário.
