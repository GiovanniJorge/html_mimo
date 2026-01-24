![Preview do projeto](preview.png)

# Caesar Cipher

Demo online: [https://giovannijorge.github.io/html-mimo/projetos/caesar-cipher/](https://giovannijorge.github.io/html-mimo/projetos/caesar-cipher/)

Descrição
--------
Este é um projeto simples demonstrando a cifra de César (Caesar cipher) implementada em HTML, CSS e JavaScript. A aplicação permite cifrar e decifrar textos usando um deslocamento (shift) configurável. Foi criada como exercício educacional e como exemplo prático de manipulação de strings e DOM.

Funcionalidades
--------------
- Cifrar texto com deslocamento configurável (0–25).
- Decifrar texto aplicando o deslocamento inverso.
- Mantém capitalização das letras.
- Caracteres não alfabéticos (como números, pontuação e espaços) são preservados.
- Interface simples e responsiva para testar rapidamente a cifra.

Como usar
--------
1. Abra o arquivo `index.html` localmente no navegador ou acesse a demo online:
   - [https://giovannijorge.github.io/html-mimo/projetos/caesar-cipher/](https://giovannijorge.github.io/html-mimo/projetos/caesar-cipher/)
2. Insira o texto no campo de entrada.
3. Ajuste o valor do deslocamento (shift) entre 0 e 25.
4. Escolha entre "Cifrar" ou "Decifrar".
5. Veja o resultado no campo de saída e copie conforme necessário.

Como funciona
---------------------
A cifra de César desloca cada letra do alfabeto por um valor fixo (shift). Por exemplo, com shift = 3:
- A → D
- B → E
- Z → C (wrap-around)

Regras aplicadas:
- Apenas letras A–Z / a–z são deslocadas.
- Maiúsculas e minúsculas são mantidas.
- Outros caracteres permanecem inalterados.

Exemplos
--------
Entrada: `Hello, World!` (shift = 3)  
Saída (cifrada): `Khoor, Zruog!`

Entrada: `ABC` (shift = 1)  
Saída: `BCD`

Arquivos principais
-------------------
- `index.html` — interface do usuário.
- `style.css` — estilos e layout.
- `script.js` — lógica de cifra (cifrar/decifrar, manipulação do DOM).
- `preview.png` — imagem de preview usada neste README.

Tecnologias
-----------
- HTML5
- CSS3
- JavaScript (vanilla)

Acessibilidade e boas práticas
------------------------------
- Campos de formulário com labels para compatibilidade com leitores de tela.
- Contraste de cores com atenção à legibilidade.
- Uso mínimo de bibliotecas externas para facilitar estudo e entendimento do código.

Contribuição
------------
Contribuições são bem-vindas. Sugestões:
- Melhorar testes e cobertura de casos (acentos, alfabetos estendidos).
- Implementar suporte para outros alfabetos ou modos (ROT13, por exemplo).
- Adicionar opção para preservar ou remover acentos antes do processamento.

Para contribuir:
1. Fork este repositório.
2. Crie uma branch com sua feature: `git checkout -b minha-feature`.
3. Faça commits descritivos.
4. Abra um Pull Request descrevendo as mudanças.

Licença
-------
Nenhuma licença específica foi adicionada a este repositório por enquanto. Se desejar, adicione um arquivo `LICENSE` (por exemplo MIT) para permitir reuso explícito.

Autor
-----
Giovanni Jorge — repositório principal: [GiovanniJorge/html-mimo](https://github.com/GiovanniJorge/html-mimo)

Contato
-------
Problemas, dúvidas ou sugestões podem ser abertas como issues no repositório ou enviadas via perfil do GitHub.
