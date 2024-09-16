# Calculadora de Gorjeta

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="1000">

Este é um aplicativo de calculadora de gorjeta desenvolvido usando .NET MAUI e C#. O objetivo do aplicativo é ajudar os usuários a calcular a gorjeta e o valor total da conta de maneira rápida e fácil.

## Funcionalidades

### 1. **Entrada do Valor da Conta**

- O usuário pode inserir o valor total da conta no campo de texto designado. O aplicativo calcula a gorjeta e o valor total com base nessa entrada.

### 2. **Seleção da Porcentagem da Gorjeta**

- **Slider de Porcentagem**: Um controle deslizante (`TipSlider`) permite ao usuário ajustar a porcentagem da gorjeta. A porcentagem selecionada é exibida em um rótulo (`TipPercentLabel`).
- **Botões de Porcentagem Predefinida**: Dois botões estão disponíveis para definir rapidamente a porcentagem da gorjeta para valores predefinidos (15% e 20%). Ao clicar em um desses botões, o valor do slider é ajustado automaticamente e o rótulo da porcentagem é atualizado.

### 3. **Arredondamento dos Valores**

- **Arredondar para Cima**: Um botão (`RoundUpButton`) arredonda o valor da gorjeta e o valor total da conta para cima. O valor arredondado é exibido nos rótulos correspondentes.
- **Arredondar para Baixo**: Um botão (`RoundDownButton`) arredonda o valor da gorjeta e o valor total da conta para baixo. O valor arredondado é exibido nos rótulos correspondentes.

### 4. **Atualização Dinâmica dos Valores**

- **Alteração da Porcentagem da Gorjeta**: Quando o usuário ajusta o slider de porcentagem, o aplicativo recalcula e atualiza automaticamente o valor da gorjeta e o valor total da conta.
- **Alteração do Valor da Conta**: Sempre que o valor da conta é alterado, o aplicativo recalcula a gorjeta e o valor total com base na porcentagem selecionada e atualiza a interface com os novos valores.

## Estrutura do Código

- **Variáveis Globais**:
  - `valorTotal`: Armazena o valor total da conta, incluindo a gorjeta.
  - `valorDaGorjeta`: Armazena o valor calculado da gorjeta.
  - `valor`: Armazena o valor inicial da conta (sem a gorjeta).

- **Eventos e Funções**:
  - `SetLowTip_Clicked`: Define a porcentagem da gorjeta para 15%.
  - `SetHighTip_Clicked`: Define a porcentagem da gorjeta para 20%.
  - `RoundUpButton_Clicked`: Arredonda os valores da gorjeta e do total para cima.
  - `RoundDownButton_Clicked`: Arredonda os valores da gorjeta e do total para baixo.
  - `TipSlider_ValueChanged`: Atualiza a porcentagem da gorjeta e recalcula os valores ao alterar o slider.
  - `AmountEntry_TextChanged`: Recalcula a gorjeta e o total sempre que o valor da conta é alterado.

## Requisitos

- .NET MAUI
- C#

## Como Executar o Aplicativo

1. Clone o repositório para a sua máquina local.
2. Abra o projeto no Visual Studio com suporte ao .NET MAUI.
3. Compile e execute o aplicativo no simulador ou dispositivo de sua escolha.

## Créditos

Desenvolvido por Mateus S. & Guilherme Barros

- GitHub: [Matz-Turing](https://github.com/Matz-Turing)
- GitHub: [guilherme-barros](https://github.com/guilherme-barros)
