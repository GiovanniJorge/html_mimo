# Rick and Morty

![Preview do projeto](preview.png)

Demo online: [https://giovannijorge.github.io/html-mimo/projetos/rick-and-morty/](https://giovannijorge.github.io/html-mimo/projetos/rick-and-morty/)

Descrição
--------
Rick and Morty Explorer é um pequeno projeto em HTML, CSS e JavaScript que consome a API pública Rick and Morty (https://rickandmortyapi.com/) para listar personagens da série. A aplicação permite buscar, filtrar e visualizar detalhes de personagens com uma interface simples e responsiva — ideal como exercício de consumo de APIs, manipulação do DOM e boas práticas front-end.

Funcionalidades
--------------
- Listagem de personagens com imagens e informações básicas (nome, status, espécie).
- Busca por nome (consulta em tempo real ou por envio).
- Filtros por status, espécie e gênero.
- Paginação (navegação entre páginas de resultados da API).
- Visualização de detalhes do personagem em modal ou painel (localização, episódios, etc.).
- Tratamento de erros e estados (carregando, sem resultados).
- Layout responsivo para mobile e desktop.

Como usar
--------
1. Abra o arquivo `index.html` localmente no navegador ou acesse a demo online:
   - [https://giovannijorge.github.io/html-mimo/projetos/rick-and-morty/](https://giovannijorge.github.io/html-mimo/projetos/rick-and-morty/)
2. Use o campo de busca para pesquisar por nome de personagem.
3. Ajuste os filtros por status, espécie ou gênero conforme desejado.
4. Navegue entre páginas usando os controles de paginação.
5. Clique em uma carta (card) de personagem para ver informações detalhadas.

Como funciona
-------------
A aplicação faz requisições à API pública Rick and Morty usando fetch:
- Endpoint principal: `https://rickandmortyapi.com/api/character`
- Parâmetros usados: `name`, `status`, `species`, `gender`, `page`
- Os resultados retornados são processados e renderizados dinamicamente como um grid de cards.
- Ao abrir um card, a aplicação exibe detalhes adicionais (por exemplo, lista de episódios) requisitando, quando necessário, endpoints adicionais da API.

Boas práticas aplicadas:
- Separação de responsabilidades entre HTML, CSS e JavaScript.
- Estados de carregamento e mensagens de erro claras.
- Uso do atributo `alt` em imagens para acessibilidade.
- Layout responsivo e botões e inputs com labels para leitores de tela.

Exemplos
--------
- Buscar por nome:
  - Entrada: `rick`
  - Resultado: lista com personagens cujo nome contém "rick" (por exemplo, "Rick Sanchez").
- Filtrar por status:
  - Selecionar `Alive` mostrará apenas personagens com status vivo.
- Paginação:
  - Navegue para a próxima página para carregar mais personagens retornados pela API.

Arquivos principais
-------------------
- `index.html` — interface do usuário.
- `style.css` — estilos e layout responsivo.
- `script.js` — lógica de consumo da API, filtros, paginação e manipulação do DOM.
- `preview.png` — imagem de preview usada neste README.

Tecnologias
-----------
- HTML5
- CSS3
- JavaScript (vanilla)
- Fetch API
- Rick and Morty API (https://rickandmortyapi.com/)

Acessibilidade e boas práticas
------------------------------
- Labels em campos de formulário para compatibilidade com leitores de tela.
- Contraste e tamanhos de fonte pensados para legibilidade.
- Indicação clara de estados (carregando / erro / sem resultados).
- Uso mínimo de bibliotecas externas para facilitar estudo e entendimento do código.

Possíveis melhorias
-------------------
- Implementar cache local (localStorage) para reduzir requisições na mesma sessão.
- Adicionar filtragem mais avançada (ordenar por nome, filtrar por múltiplos critérios combinados).
- Suporte a pesquisa com debounce para reduzir chamadas à API durante digitação.
- Paginação infinita (infinite scroll) como alternativa aos controles atuais.
- Testes automatizados (unitários / E2E) para a lógica de busca e renderização.

Contribuição
------------
Contribuições são bem-vindas. Sugestões:
- Corrigir bugs ou melhorar tratamento de erros.
- Implementar uma das melhorias sugeridas acima.
- Melhorar acessibilidade e responsividade.

Para contribuir:
1. Fork este repositório.
2. Crie uma branch com sua feature: `git checkout -b minha-feature`.
3. Faça commits descritivos.
4. Abra um Pull Request descrevendo as mudanças.

Licença
-------
Nenhuma licença específica foi adicionada a este repositório por enquanto. Se desejar permitir reuso explícito, adicione um arquivo `LICENSE` (por exemplo MIT).

Autor
-----
Giovanni Jorge — repositório principal: [GiovanniJorge/html-mimo](https://github.com/GiovanniJorge/html-mimo)

Contato
-------
Problemas, dúvidas ou sugestões podem ser abertas como issues no repositório ou enviadas via perfil do GitHub.
```
