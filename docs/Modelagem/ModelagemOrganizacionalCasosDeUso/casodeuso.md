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


## Casos de Uso

<center>

<font size="2"><p style="text-align: center">Tabela x: </p></font>

| UC01 |  Buscar Veiculo |
| -: | :- |
| **Atores** | Usuário |
| **Funcionalidade** | O usuário pode fazer uma busca pelo veiculo desaparecido |
| **Pré-condições** | Conexão com a internet, Login no sistema |
| **Ação** | O usuário busca um veiculo  |
| **Fluxo básico** | <ul><li> O usuário acessa o aplicativo. </br> <ul><li> O usuário acessa a aba veiculo. </br> <ul><li> O usuário faz a busca pelo veículo </br> |
| **Fluxos alternativos** | <ul><li> O usuário acessa o aplicativo </br> <ul><li> O usuário acessa a aba veiculo. </br> <ul><li> O app solicita a localização do usuário </br> <ul><li> O usuário seleciona "Sim"</br>  |
| **Fluxos de exceção** | <ul><li> O usuário acessa o aplicativo </br> <ul><li> O usuário acessa a aba veiculo. </br> <ul><li>  O usuário faz a busca pelo veículo. </br> <ul><li> O aplicativo apresenta "Dados Incorretos" </br>  |
| **Pós-condições** |POS01. O usuário tem acesso aos dados sobre o veiculo. |
| **Data da criação** | 23/11/2024 |
| **Rastreabilidade** | |

<font size="2"><p style="text-align: center">Autor: [Italo Bruno](https://github.com/ItaloBrunoM)  .</p></font>

</center>

<center>

<font size="2"><p style="text-align: center">Tabela x: </p></font>

| UC02 |  Gerenciar Jogador |
| -: | :- |
| **Atores** | Treinador |
| **Funcionalidade** | O treinador de um time pode gerenciar os jogadores do seu time |
| **Pré-condições** | Conexão com a internet, Login no sistema com o perfil de treinador, Treinador deve estar associado a pelo menos um time no sistema |
| **Ação** | "O treinador gerencia seus jogadores, podendo visualizar, cadastrar, editar ou excluir informações relacionadas a eles."  |
| **Fluxo básico** | <ul><li> O usuário acessa o aplicativo como treinador. </br> <ul><li> O treinador acessa seu time. </br> <ul><li> O sistema exibe a lista de jogadores associados ao time e informações do time. </br> <ul><li> O treinador pode realizar uma das ações disponíveis no gerenciamento de jogadores: Visualizar, Adicionar, Editar e Excluir </br>|
| **Fluxos alternativos** | <ul><li> O treinador tenta acessar um time, mas ainda não possui times cadastrados </br> <ul><li> O sistema exibe uma mensagem informando que ele deve primeiro criar um time."</br>  |
| **Fluxos de exceção** | <ul><li> O treinador busca um jogador pelo nome, mas o jogador não está na lista</br> <ul><li>O sistema exibe uma mensagem indicando "Nenhum jogador encontrado."</br> |
| **Pós-condições** |<ul><li> POS01. As alterações feitas no gerenciamento de jogadores são salvas no banco de dados</br> <ul><li> POS02. O treinador visualiza a lista atualizada de jogadores. |
| **Data da criação** | 23/11/2024 |
| **Rastreabilidade** | |

<font size="2"><p style="text-align: center">Autor: [Artur Jackson](https://github.com/artur-jack)  .</p></font>

</center>

## Diagrama de Casos de Uso

## Bibliografia

## Histórico de Versão

|Versão|Data|Descrição|Autor|Revisor| Detalhes da revisão |
|:----:|----|---------|-----|:-------:|-----| 
|  |  |  |  |  | |