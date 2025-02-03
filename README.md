# Tarefa: Exibição de Dígitos com LEDs RGB 💡

Este projeto foi desenvolvido para controlar LEDs RGB e exibir números de 0 a 9 em um display utilizando a placa Raspberry Pi Pico, com a ajuda da biblioteca PIO para controle de LEDs e interrupções para modificar o número exibido.

## Arquivos do Projeto 📁
- **main.c**: Código principal que gerencia a exibição dos números e o controle dos LEDs.
- **diagram.json**: Arquivo de configuração do projeto para visualização e simulação no Wokwi.
- **pio_archive.h**: Biblioteca de suporte para as funções de controle dos LEDs através da tecnologia PIO.

## Descrição do Projeto 📜
Este projeto utiliza LEDs RGB para exibir números de 0 a 9. A exibição dos números é realizada por meio de uma sequência de frames, com diferentes combinações de cores RGB. O usuário pode alterar o número exibido por meio de botões de interrupção, permitindo incrementar ou decrementar o número entre 0 e 9.

## Funcionalidades principais 🔧
- **Contagem de 0 a 9**: O número exibido é alterado conforme a interação com os botões configurados para incrementar e decrementar o valor.
- **Cores RGB**: Cada número é exibido com uma combinação única de cores RGB, e a intensidade das cores pode ser ajustada.
- **Controle de LEDs**: Utilizando a tecnologia PIO, é possível controlar a intensidade e as cores dos LEDs.
- **Botões de interrupção**: Usados para modificar o número exibido.

## Estrutura do Código 🧑‍💻
- **Função RGB()**: Calcula a cor RGB de acordo com os valores de brilho e intensidade fornecidos.
- **Função DESENHO()**: Controla a exibição do número utilizando um conjunto de frames com os valores RGB.
- **Função gpio_irq_handler()**: Função de interrupção que trata os eventos dos botões para alterar o número exibido.

## Funcionalidade de Interrupção 🔄
O código responde a interrupções geradas pelos botões **BA** (incrementa) e **BB** (decrementa). Cada pressão de botão altera o número exibido no display de LEDs RGB, permitindo ao usuário navegar de 0 a 9.

## Simulação no Wokwi 🌐
O projeto foi simulado na plataforma Wokwi, permitindo testar o funcionamento do código sem a necessidade de hardware físico.

[Link para o vídeo de explicação no YouTube 📺](https://youtu.be/Bo8D-CeOW4c?si=i-t5zmAkYxG6X4yT))
[Link para a simulação na plataforma Wokwi 🤖](https://wokwi.com/projects/421833036248849409)

## Requisitos de Hardware 🖥️
- **Raspberry Pi Pico**: Placa de microcontrolador.
- **LEDs RGB**: Utilizados para exibir os números.
- **Botões**: Para incrementar e decrementar o número.
- **Resistores**: Para proteção dos LEDs.

## Como Executar 🏃‍♂️
1. Baixe o código para o seu Raspberry Pi Pico.
2. Compile o código utilizando o compilador C adequado.
3. Faça upload do código para a placa.
4. Conecte os LEDs RGB nos pinos definidos no código.
5. Pressione os botões para alterar o número exibido.
6. Ou, baixe a abra os arquivos pelo Wokwi, e o funcionamento seguirá o do link acima.
