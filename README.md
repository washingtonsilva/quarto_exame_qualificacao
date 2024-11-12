# Template para Exame de Qualificação - IFMG

Template em Quarto para elaboração do documento de Exame de 
Qualificação do Mestrado Profissional em Administração do IFMG - 
Campus Formiga.

## Estrutura do Projeto

O template contém os seguintes arquivos essenciais[2]:

- `exame_qualificacao.qmd`: Arquivo principal do Quarto contendo a 
estrutura lógica do documento.

- `pre_textuais.tex`: Template LaTeX para geração da capa e resumo.

- `referencias.bibtex`: Arquivo para gerenciamento das 
referências bibliográficas.

- `associacao-brasileira-de-normas-tecnicas-ipea.csl`: Arquivo de 
estilo ABNT 2023.

## Como Usar

### Pré-requisitos

- Quarto (versão mais recente)
- Editor de texto (RStudio)
- Sistema TeX instalado (tinytex recomendado)
- linguagem R ou Python instaladas.

### Utilizando o Template

1. Clique no botão "Use this template" no topo da página
2. Clone o novo repositório criado
3. Edite o arquivo `exame_qualificacao.qmd` com seu conteúdo
4. Personalize o arquivo `pre_textuais.tex` com suas informações
5. Adicione suas referências no arquivo `referencias.bibtex`

### Gerando o PDF

Clique em `Render` ou utilize o terminal

```bash
quarto render exame_qualificacao.qmd
```

## Estrutura do Documento

O template gera um documento PDF com a seguinte estrutura[3]:

- Capa (personalizada para o IFMG)
- Resumo
- Sumário
- Introdução
  - Justificativa
  - Objetivos
- Revisão de Literatura
- Metodologia
- Resultados Esperados
- Cronograma
- Referências
- Apêndices

## Personalização

### Capa e Elementos Pré-textuais

Para personalizar a capa e o resumo, edite o arquivo 
`pre_textuais.tex` alterando:

- Nome do autor
- Título e subtítulo
- Orientador e coorientador
- Linha de pesquisa
- Texto do resumo
- Palavras-chave

### Formatação

O documento está configurado com:

- Papel A4
- Margens: superior 3cm, inferior 2cm, esquerda 3cm, direita 2cm
- Fonte tamanho 12pt
- Espaçamento entre linhas 1.25
- Parágrafos indentados
- Numeração automática de seções

## Licença

Este template está sob a licença MIT.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para:

- Reportar bugs
- Sugerir melhorias
- Enviar pull requests

## Atualizações e Versões

Este template está em desenvolvimento contínuo para garantir 
conformidade com as normas mais recentes e melhorar a 
experiência dos mestrandos.

### Como se Manter Atualizado

- **Observando o Repositório**: Clique no botão "Watch" no topo 
da página para receber notificações sobre novas versões e atualizações.

- **Verificando Releases**: Novas versões serão publicadas como 
releases no GitHub, incluindo notas detalhadas sobre as mudanças.

### Atualizando Seu Projeto

Se você já está usando o template, há duas opções para atualização:

1. **Para Projetos Novos**:

   - Sempre utilize a versão mais recente do template através 
   do botão "Use this template"


2. **Para Projetos em Andamento**:
   - Você pode sincronizar seu repositório com o template original
   - Alternativamente, pode aplicar manualmente as alterações 
     consultando o histórico de mudanças

### Changelog

Mantenha-se informado sobre as alterações consultando:

- O arquivo CHANGELOG.md no repositório
- A seção de Releases no GitHub
- As discussões e issues relacionadas a atualizações

## Suporte

Em caso de dúvidas ou problemas, abra uma issue no repositório.


