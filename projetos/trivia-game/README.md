# Trivia Game

![Preview do projeto](preview.png)

Demo online: [https://giovannijorge.github.io/html-mimo/projetos/trivia-game/](https://giovannijorge.github.io/html-mimo/projetos/trivia-game/)

Descrição
--------
Trivia Game é um pequeno projeto em HTML, CSS e JavaScript que implementa um jogo de perguntas e respostas (quiz). A aplicação permite selecionar categoria, dificuldade e número de perguntas, traz um temporizador por questão, calcula pontuação e exibe um resumo ao final — ideal como exercício de lógica, consumo de APIs, manipulação do DOM e boas práticas de front-end.

Funcionalidades
--------------
- Busca/geração de perguntas (via API pública Open Trivia DB ou conjunto local de perguntas).
- Seleção de categoria, dificuldade e quantidade de perguntas.
- Apresentação de alternativas embaralhadas (múltipla escolha).
- Temporizador por pergunta com feedback visual.
- Registro de acertos, erros e pontuação final.
- Visualização do resultado e revisão de respostas corretas ao finalizar.
- Tratamento de estados (carregando, erro na requisição, sem perguntas).
- Layout responsivo para mobile e desktop.

Como usar
--------
1. Abra o arquivo `index.html` localmente no navegador ou acesse a demo online:
   - [https://giovannijorge.github.io/html-mimo/projetos/trivia-game/](https://giovannijorge.github.io/html-mimo/projetos/trivia-game/)
2. Escolha a categoria, dificuldade e o número de perguntas desejado.
3. Clique em "Iniciar jogo" para carregar as perguntas.
4. Responda cada pergunta antes que o tempo acabe — o temporizador é visível em cada rodada.
5. Ao final, veja sua pontuação e reveja as respostas corretas.

Como funciona
-------------
A aplicação pode requisitar perguntas da Open Trivia Database (https://opentdb.com/) usando parâmetros:
- `amount` — número de perguntas
- `category` — categoria (opcional)
- `difficulty` — dificuldade (easy, medium, hard)
- `type` — tipo da pergunta (multiple)

Fluxo principal:
- O usuário escolhe as opções e envia o formulário.
- `script.js` faz a requisição (fetch) para obter as perguntas.
- Perguntas e alternativas são processadas e renderizadas dinamicamente.
- Em cada pergunta é iniciado um temporizador; o jogador escolhe uma alternativa ou o tempo expira.
- Resultados (acertos, erros, pontuação) são acumulados e apresentados ao final.

Boas práticas aplicadas:
- Separação de responsabilidades entre HTML, CSS e JavaScript.
- Estados de carregamento e mensagens de erro claras.
- Uso de atributos `aria-` e `alt` para melhorar acessibilidade.
- Layout responsivo e controles acessíveis por teclado.

Exemplos
--------
- Iniciar uma partida com 10 perguntas de dificuldade "medium".
  - Selecionar `10` em quantidade e `Medium` em dificuldade, depois "Iniciar jogo".
- Temporizador:
  - Cada pergunta tem, por exemplo, 30 segundos; se o tempo acabar a pergunta é marcada como incorreta e o jogo avança.
- Revisão de respostas:
  - Ao terminar, o resumo mostra cada pergunta, sua escolha e a resposta correta.

Arquivos principais
-------------------
- `index.html` — interface do usuário.
- `style.css` — estilos e layout responsivo.
- `script.js` — lógica do jogo: requisição de perguntas, temporizador, pontuação e manipulação do DOM.
- `preview.png` — imagem de preview usada neste README.

Tecnologias
-----------
- HTML5
- CSS3
- JavaScript (vanilla)
- Fetch API
- Open Trivia Database (opentdb.com) — opcional, a aplicação suporta fallback para perguntas locais

Acessibilidade e boas práticas
------------------------------
- Labels e roles em campos de formulário para compatibilidade com leitores de tela.
- Destaque visual claro no foco para navegação por teclado.
- Contraste e tamanhos de fonte pensados para legibilidade.
- Indicação clara de estados (carregando / erro / sem perguntas).
- Alternativas de cores para o temporizador e feedback de acerto/erro.

Contribuição
------------
Contribuições são bem-vindas. Sugestões:
- Adicionar persistência de pontuação (localStorage) e placar global.
- Implementar modos de jogo (por tempo total, por rounds).
- Melhorar UX com animações acessíveis e som (com opção de desativar).
- Internacionalização / suporte a múltiplos idiomas.
- Testes automatizados para a lógica do jogo.

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
