# repositorio_modelo
O nome do repostório deve ser o mesmo do projeto. Por exemplo: Projeto Siga 
## Boas praticas
- todo read me precisa informar:
- visão geral do projeto
- as tecnologias utilizadas
- como instalar ou utilizar esse projeto
- quem contirubuiu? (equipe)
- como pode contribuir? (comunidade externa que vê o seu repositorio publico )

## Organização de pastas
- Toda linguagem de programação exige uma organização em pastas. Em comum todas tem essa estrutura:
  - /src -> pasta indicada para colocar o código fonte do projeto
  - /teste -> A pasta indicada para colocar os testes unitarios
  - /public -> A pasta é indicada pra colocar o front-en dou qualquer arquivo que precisa ficar a nível publico. A nivel API, teriamos os ENDPOINTs (Rotas de acesso)
  - /config -> (ou scripts) arquivos de configuração ou intalação de bibliotecas do projeto (isso também pode ficar na raiz do projeto - é uma pasta opcional)
  - /docs -> pasta é indicada para guardar imagens ou docs relacionadas ao projeto. Por exemplo: Diagramas, Fluxogramas, etc

## Utilizar boas práticas e commits 
- É necessario realizar os dois:
    - Commit Atômico: realizar commits pequenos -> a unidade de trabalho
    - commit Semantico: É informar com sufixo e em poucas palavras o que foi realizados nessa unidade de trabalho 

## Na raiz do projeto 
- deve ter:
    - .gitignore: é utilizado para informar ao git quais extensões ou pastas devem ser ignoradas
    - licese: é informado qual é a licença do projeto (Obrigatorio quando o projeto é publico) 
    - contributing: é informado quem são os autores e como contribuir
    - changelog: é utilizado para informar o Histórico de Versões do projeto

## Gerenciar branchs 
- um projeto deve ter algumas dessas branchs abaixo:
    - main(master): Versão estável do projeto (ou aquilo que o publico está utilizando no momento)
    - homolog: 
        - Versão posterior a de desenvolvimento, ou seja, é a de testes. Antecipa a main 
    - develop:
        - Versão em desenvolvimento, normalmente é utilizado por Desenvolvedores do projeto.
        - Centralizadora das modificações realizadas pelos devs
    - branchs relacionadas ao card do kanban:
        - Por exemplo -> [sulfixo-atomico]/[nome-card]
        - Cada card do kanban vai ter uma branch
        - Cada dev pega um ou N cards do kanban
        - Cada branch é baseada na develop
        - No final é mesclada a develop

    - Flow das branchs:
        - branch-de-trabalho -> develop -> homolog -> main
