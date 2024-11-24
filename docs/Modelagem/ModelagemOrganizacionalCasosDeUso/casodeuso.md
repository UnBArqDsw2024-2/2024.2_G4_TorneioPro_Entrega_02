# Casos de Uso

## Introdução

## Metodologia
O diagrama de caso de uso é uma representação visual que sintetiza as interações entre os usuários e o sistema. Para definir os casos de uso do nosso sistema, realizamos uma reunião no Discord, durante a qual analisamos detalhadamente as funcionalidades previstas para o nosso site. Essa abordagem nos permitiu identificar cenários realistas de uso, mapeando as principais funcionalidades e as interações entre os usuários e o sistema que estamos desenvolvendo. Como resultado, conseguimos uma visão clara e organizada dos requisitos, o que facilitará a implementação.

<font size="2"><p style="text-align: center">Tabela 1: Elementos usados no diagrama de casos de uso </p></font>

| Nome           |Descrição                     |    Representação                           |
|----------------|------------------------------|--------------------------------------------|
| Ator           | Entidade externa que interage com o sistema, podendo ser um usuário ou outro sistema. No nosso caso, utilizamos quatro atores, organizador, treinador, jogador e o próprio sistema. | ![Ator](../../Assets/ator.jpeg) |
|Retângulo | Representação do sistema por inteiro |![Retângulo](../../Assets/retangulo.jpeg)|
|Seta| Representações das interações entre atores e usos no sistema|![Setas](../../Assets/setas.jpeg)|
|Elipse|Representação dos casos de uso. Um caso de uso mostra uma funcionalidade ou ação a ser realizada dentro do sistema.|![Elipse](../../Assets/elipse.jpeg)|

<font size="2"><p style="text-align: center">Autor: [Flávio Melo](https://github.com/flavioovatsug)</p></font>

## Diagrama de Casos de Uso

<font size="2"><p style="text-align: center">Figura 1: Diagrama de Casos de Uso</p></font>

![Diagrama de Casos de Uso](../../Assets/diagramaCasosDeUso.jpg)

<font size="2"><p style="text-align: center">Autor: [Squad 2](### COLOCAR LINK ###) e [Squad 3](### COLOCAR LINK ###)</p></font>

## Casos de Uso

<center>

<font size="2"><p style="text-align: center">Tabela 1: </p></font>

| UC01 |  Gerenciar Torneio |
| -: | :- |
| **Atores** | Organizador |
| **Funcionalidade** | O organizador pode criar e gerenciar torneios |
| **Pré-condições** | Conexão com a internet, Login no sistema como organizador |
| **Ação** | "O Organizador gerencia o campeonato, podendo visualizar, cadastrar, editar ou excluir informações relacionadas."  |
| **Fluxo básico** | <ul><li> O usuário acessa o aplicativo como organizador. </br> <ul><li> O organizador acessa os torneios. </br> <ul><li> O sistema exibe a lista de torneios. </br> <ul><li> O organizador pode realizar uma das ações disponíveis no gerenciamento de jogadores: Criar, Visualizar, Adicionar, Editar e Excluir </br> |
| **Fluxos alternativos** | <ul><li>O organizador acessa a funcionalidade de torneios.</li><li>O sistema exibe uma mensagem informando "Nenhum torneio encontrado".</li><li>O sistema apresenta a opção "Criar Torneio".</li><li>O organizador clica na opção "Criar Torneio".</li><li>O sistema exibe o formulário de criação de torneio.</li><li>O organizador insere os dados obrigatórios e confirma a criação.</li><li>O sistema salva o novo torneio no banco de dados e exibe a lista de torneios atualizada.</li></ul> |
| **Fluxos de exceção** | <ul><li> O usuário acessa o aplicativo como organizador. </br> <ul><li> O organizador cria um torneio sem colocar nenhum dado</br> <ul><li>O sistema exibe uma mensagem indicando "Faltam informações obrigatórias."</br>  |
| **Pós-condições** |<ul><li> POS01. As alterações feitas no gerenciamento de torneio são salvas no banco de dados</br> |
| **Data da criação** | 23/11/2024 |
| **Rastreabilidade** | |

<font size="2"><p style="text-align: center">Autor: [Italo Bruno](https://github.com/ItaloBrunoM)  .</p></font>

</center>

<center>

<font size="2"><p style="text-align: center">Tabela 2: </p></font>

| UC02 |  Gerenciar Jogador |
| -: | :- |
| **Atores** | Treinador |
| **Funcionalidade** | O treinador de um time pode gerenciar os jogadores do seu time |
| **Pré-condições** | Conexão com a internet, Login no sistema com o perfil de treinador, Treinador deve estar associado a pelo menos um time no sistema |
| **Ação** | "O treinador gerencia seus jogadores, podendo visualizar, cadastrar, editar ou excluir informações relacionadas a eles."  |
| **Fluxo básico** | <ul><li> O usuário acessa o aplicativo como treinador. </br> <ul><li> O treinador acessa seu time. </br> <ul><li> O sistema exibe a lista de jogadores associados ao time e informações do time. </br> <ul><li> O treinador pode realizar uma das ações disponíveis no gerenciamento de jogadores: Visualizar, Adicionar, Editar e Excluir </br>|
| **Fluxos alternativos** | <ul><li> O treinador tenta acessar um time, mas ainda não possui times cadastrados </br> <ul><li> O sistema exibe uma mensagem informando que ele deve primeiro criar um time."</br>  |
| **Fluxos de exceção** | <ul><li> O treinador busca um jogador pelo nome, mas o jogador não está na lista</br> <ul><li>O sistema exibe uma mensagem indicando "Nenhum jogador encontrado."</br> |
| **Pós-condições** | <ul><li> POS02. As alterações feitas no gerenciamento de jogadores são salvas no banco de dados</br> <ul><li> O treinador visualiza a lista atualizada de jogadores. |
| **Data da criação** | 23/11/2024 |
| **Rastreabilidade** | |

<font size="2"><p style="text-align: center">Autor: [Artur Jackson](https://github.com/artur-jack)  .</p></font>

</center>

<center>

<font size="2"><p style="text-align: center">Tabela 3: </p></font>

| UC03 |  Encerrar Campeonato |
| -: | :- |
| **Atores** | Organizador |
| **Funcionalidade** | O organizador pode encerrar campeonatos após sua conclusão |
| **Pré-condições** | Conexão com a internet, Login no sistema como organizador, Campeonato deve estar ativo |
| **Ação** | "O Organizador encerra o campeonato, impedindo edições futuras e atualizando o status para encerrado."  |
| **Fluxo básico** | <ul><li> O organizador acessa o aplicativo como organizador. </br> <ul><li> O organizador navega até a seção de campeonatos. </br> <ul><li> O sistema exibe a lista de campeonatos ativos. </br> <ul><li> O organizador seleciona o torneio desejado e clica na opção "Encerrar Campeonato". </br> <ul><li> O sistema solicita confirmação para encerrar. </br> <ul><li> O organizador confirma a ação. </br> <ul><li> O sistema atualiza o status do campeonato para "Encerrado" e impede edições futuras. |
| **Fluxos alternativos** | <ul><li> O organizador tenta acessar a funcionalidade de encerrar um campeonato que já está encerrado. <ul><li> O sistema não mostra a opção de encerrar  |
| **Fluxos de exceção** | <ul><li> O organizador tenta encerrar um campeonato, mas há pendências no sistema (ex.: resultados não cadastrados). </br> <ul><li> O sistema exibe uma mensagem indicando: "Não é possível encerrar o campeonato. Resolva as pendências antes de prosseguir." </br> |
| **Pós-condições** |<ul><li> POS01. O status do campeonato é atualizado para "Encerrado" no banco de dados. </br> <ul><li> POS02. O campeonato é exibido na lista de históricos encerrados. |
| **Data da criação** | 24/11/2024 |
| **Rastreabilidade** |  |


<font size="2"><p style="text-align: center">Autor: [Yan Werlley](https://github.com/YanWerlley).</p></font>

</center>

<center>

<font size="2"><p style="text-align: center">Tabela 4: </p></font>

| **UC04** | **Gerenciar Time** |
|----------|--------------------|
| **Atores** | Treinador |
| **Funcionalidade** | O Treinador pode criar e mudar as características do time. |
| **Pré-condições** | - Conexão com a internet<br>- Login no sistema como treinador |
| **Ação** | O treinador gerencia seus times, podendo visualizar, cadastrar, editar ou excluir informações relacionadas a eles. |
| **Fluxo básico** | <ul><li>O usuário acessa o app como treinador.</li><li>O treinador navega até a seção de times.</li><li>O sistema exibe a lista de times ativos do treinador.</li><li>O treinador seleciona a opção "Criar time".</li><li>Excluir Time (FA01).</li><li>Editar Time (FA02).</li><li>O sistema mostra as informações necessárias a serem preenchidas.</li><li>O treinador preenche as informações.</li><li>O sistema valida as informações.</li><li>O sistema salva as informações do time.</li></ul> |
| **Fluxos alternativos** | <ul><li>**FA01 – Excluir time**<ul><li>O treinador seleciona o ícone de lixeira.</li><li>O sistema exige a confirmação da ação de excluir.</li><li>O treinador confirma a exclusão clicando em "deletar".</li><li>O sistema exclui o time.</li><li>Fim do FA01.</li></ul></li><li>**FA02 – Editar time**<ul><li>O treinador seleciona o ícone de lápis.</li><li>O sistema mostra as informações necessárias a serem preenchidas.</li><li>O treinador preenche as informações.</li><li>O sistema valida as informações.</li><li>O sistema salva as informações do time.</li><li>Fim do FA02.</li></ul></li></ul> |
| **Fluxos de exceção** | <ul><li>**FE01** - O treinador tenta criar um time mas não preenche informações obrigatórias<ul><li>O sistema exibe uma mensagem indicando: "Não é possível criar o time. Por favor, preencher todos os campos."</li></ul></li><li>**FE02** - O treinador tenta editar um time mas não preenche informações obrigatórias<ul><li>O sistema exibe uma mensagem indicando: "Não é possível editar o time. Por favor, preencher todos os campos."</li></ul></li></ul> |
| **Pós-condições** | <ul><li>**POS01.** O time é criado e armazenado no banco.</li><li>**POS02.** O time é excluido da base de dados (FA01) .</li><li>**POS03.** As informações do time são atualizadas (FA02)  |
| **Data da criação** | 24/11/2024 |
| **Rastreabilidade** | - | 



<font size="2"><p style="text-align: center">Autor: [Harryson Campos](https://github.com/harry-cmartin) e [Oscar Brito](https://github.com/OscarDeBrito).</p></font>

</center>

## Diagrama de Casos de Uso

## Bibliografia

## Histórico de Versão

|Versão|Data|Descrição|Autor|Revisor| Detalhes da revisão |
|:----:|----|---------|-----|:-------:|-----| 
|  |  |  |  |  | |