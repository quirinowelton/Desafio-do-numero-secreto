# Jogo do Número Secreto 🎲

Este é um jogo simples de adivinhação em JavaScript. O objetivo é acertar o número secreto escolhido aleatoriamente pelo sistema. A cada tentativa, o jogador recebe dicas se o número é maior ou menor que o chute.

## Funcionalidades

### 1. **Escolha de Número Aleatório**
- O jogo escolhe um número secreto aleatório entre 1 e 10.
- O número é único e não se repete até que todos os números possíveis sejam sorteados.

### 2. **Interação do Jogador**
- O jogador digita um número no campo de entrada e clica em "Verificar".
- O jogo fornece feedback:
  - **Se o jogador acerta**: Exibe uma mensagem de sucesso e a quantidade de tentativas usadas.
  - **Se o jogador erra**: Indica se o número secreto é maior ou menor que o chute.

### 3. **Reinício do Jogo**
- Após o jogador acertar o número, um botão "Reiniciar" fica disponível para começar um novo jogo.
- O jogo reseta todas as variáveis, incluindo o número secreto e o contador de tentativas.

## Estrutura do Código

### Arquivos Principais
- **`index.html`**: Estrutura da interface do jogo.
- **`app.js`**: Contém toda a lógica do jogo.

### Funções

#### **1. `exibirTextoTela(tag, texto)`**
Atualiza o conteúdo de um elemento HTML com o texto fornecido.

#### **2. `mensagemInicial()`**
Exibe a mensagem inicial do jogo, incluindo o título e a instrução para o jogador.

#### **3. `verificarChute()`**
- Lê o número digitado pelo jogador.
- Compara o número com o número secreto.
- Exibe mensagens de acerto ou erro, além de dicas sobre o próximo passo.

#### **4. `numeroAleatorio()`**
- Gera um número aleatório entre 1 e 10.
- Garante que o número gerado ainda não foi usado na rodada atual.
- Reseta a lista de números sorteados quando todos os números já foram utilizados.

#### **5. `limparCampo()`**
- Limpa o campo de entrada do jogador após cada tentativa.

#### **6. `reiniciarJogo()`**
- Reinicia o jogo, resetando o número secreto, as tentativas e as mensagens exibidas na tela.

## Como Jogar

1. Abra o arquivo `index.html` em seu navegador.
2. Leia a mensagem inicial e digite um número entre 1 e 10 no campo de entrada.
3. Clique no botão "Verificar".
   - Caso acerte, uma mensagem de sucesso será exibida.
   - Caso erre, você receberá uma dica indicando se o número secreto é maior ou menor que o seu chute.
4. Quando acertar, clique no botão "Reiniciar" para começar uma nova rodada.

## Tecnologias Utilizadas

- **HTML5**: Estrutura básica da interface.
- **CSS3**: Estilo visual (não incluído no exemplo).
- **JavaScript**: Lógica do jogo e manipulação de elementos da DOM.



