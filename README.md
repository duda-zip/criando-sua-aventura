# Em Busca da Floresta Encantada

Jogo narrativo interativo desenvolvido com HTML, CSS e JavaScript, no qual as escolhas do jogador determinam os caminhos de uma aventura.

## Sobre o projeto
A história acompanha um grupo de amigos que encontra um mapa antigo indicando um tesouro escondido em uma floresta encantada.
Durante a jornada, o jogador escolhe entre diferentes caminhos, encontra um guardião mágico, explora uma caverna, atravessa um rio e pode descobrir uma vila que vive em harmonia com a natureza.
O objetivo do projeto é praticar lógica de navegação, eventos de clique e manipulação de elementos da página com JavaScript.

## Funcionalidades
- História dividida em 14 etapas.
- Escolhas por meio de botões.
- Diferentes caminhos e desfechos.
- Exibição de uma etapa por vez, sem recarregar a página.
- Imagens ilustrativas em momentos da narrativa.

## Tecnologias utilizadas
- **HTML5:** estrutura das etapas, textos, imagens e botões.
- **CSS3:** aparência da página e controle de visibilidade das etapas.
- **JavaScript:** eventos de clique e transição entre os caminhos.
- **Google Fonts:** fonte Josefin Sans.

## Como funciona
Cada botão possui um atributo `data-proximo`, que indica a próxima etapa da história.
Ao clicar, o JavaScript remove a classe `ativo` da etapa atual e aplica essa classe à etapa escolhida. O CSS utiliza essa marcação para mostrar somente o trecho correspondente.

## Organização dos arquivos
- `index.html`: narrativa, escolhas e imagens.
- `style.css`: estilos e visibilidade das etapas.
- `script.js`: lógica de navegação.
- `cenario-passo0.PNG`: imagem inicial.
- `cenario-passo4-voltar-casa.png`: imagem dos caminhos de desistência.
- `cenario-passo10-cidade-perdida.png`: imagem da vila encontrada.

## Como executar
1. Baixe e extraia o projeto.
2. Crie uma pasta chamada `img`.
3. Mova as três imagens de cenário para essa pasta, preservando os nomes e as extensões.
4. Abra `index.html` no navegador.
Não é necessário instalar dependências ou configurar um servidor. A fonte externa utiliza conexão com a internet.

## Como personalizar
Os textos e as escolhas podem ser alterados no arquivo `index.html`.
Para adicionar uma etapa, crie um elemento com a classe `passo` e um identificador exclusivo, como `passo-14`. Depois, adicione um botão em outra etapa com `data-proximo="14"`.

## Limitações atuais
- Não possui salvamento de progresso.
- Não há botão de reinício; para começar novamente, recarregue a página.
- A resolução do enigma faz parte da narrativa, sem uma pergunta para o jogador responder.
- O layout pode precisar de ajustes em telas menores.

## Aprendizados
Prática de manipulação do DOM, eventos de clique, atributos personalizados, alternância de classes CSS e organização de uma narrativa com caminhos ramificados.
