# Documentação do Projeto

Bem-vindo ao nosso projeto. Aqui você encontrará informações sobre a instalação, uso e detalhes do sistema.

# Visão Geral
O código implementado configura inicialmente os pinos do microcontrolador, especificando quais serão utilizados como entradas para receber os bits de dois conjuntos de quatro bits (`nib1` e `nib2`) e quais serão saídas para enviar os resultados da soma e o bit de transporte. Durante a execução no loop principal, o programa aguarda um sinal no pino `13` para começar a soma binária. Quando o sinal é recebido, ele lê os valores dos pinos de entrada, inicializa o bit de transporte, e calcula iterativamente a soma de cada par de bits utilizando funções específicas. Os resultados são então enviados para os pinos de saída correspondentes, permitindo que sejam utilizados por outros dispositivos ou circuitos conectados. O código opera de maneira contínua, aguardando repetidamente novos sinais no pino `13` para iniciar novas operações de soma conforme necessário.

# Instalação

Para instalar e executar o programa fornecido, siga os seguintes passos:

1. **Preparação do Ambiente de Desenvolvimento:**
   Certifique-se de ter um ambiente de desenvolvimento configurado para programar em Arduino. Isso inclui ter o Arduino IDE instalado no seu computador. Caso ainda não tenha o Arduino IDE, você pode baixá-lo gratuitamente no site oficial do Arduino e seguir as instruções de instalação para o seu sistema operacional.

2. **Abra o Arduino IDE:**
   Após instalar o Arduino IDE, abra o programa.

3. **Crie um Novo Sketch:**
   No Arduino IDE, clique em `File (Arquivo)` > `New (Novo)` para criar um novo sketch.

4. **Copie e Cole o Código:**
   Copie o código fornecido e cole no editor do Arduino IDE, substituindo o conteúdo padrão do sketch.

5. **Verifique e Compile o Código:**
   Antes de enviar o código para o Arduino, clique no botão de verificação (ícone de marca de seleção) na parte superior do IDE para verificar se não há erros de sintaxe no código.

6. **Conecte o Arduino:**
   Conecte o seu Arduino ao computador usando um cabo USB.

7. **Selecione a Placa e a Porta:**
   Vá em `Tools (Ferramentas)` > `Board (Placa)` e selecione o tipo de placa Arduino que você está usando (por exemplo, Arduino Uno).

   Em seguida, vá em `Tools (Ferramentas)` > `Port (Porta)` e selecione a porta COM à qual o Arduino está conectado.

8. **Carregue o Programa:**
   Clique no botão de upload (ícone de seta para a direita) no canto superior esquerdo do IDE para compilar e carregar o programa para o Arduino.

9. **Verifique a Execução:**
   Após o upload ser concluído com sucesso, o programa será executado no Arduino. Você pode verificar a saída usando LEDs ou outro hardware conectado aos pinos configurados no código.

Seguindo esses passos, você poderá instalar e executar o programa no seu Arduino sem problemas. Certifique-se de ajustar as conexões físicas conforme necessário, especialmente se estiver usando LEDs ou outros dispositivos de saída conforme configurado nos pinos do Arduino.

# Uso

### Para usar o software:

1. **Conexão e Configuração**: Conecte os bits dos conjuntos `nib1` e `nib2` aos pinos de entrada (`0` a `7`) e os pinos de saída (`8` a `12`) para os resultados da soma e o bit de transporte. Carregue o código no hardware usando a IDE do Arduino.

2. **Início da Operação**: O programa espera um sinal no pino `13` para começar a soma binária.

3. **Processamento da Soma**: Quando o sinal no pino `13` é recebido (`soma == 1`), ele calcula a soma dos bits utilizando funções específicas para cada bit e atualiza o bit de transporte.

4. **Saída dos Resultados**: Os resultados da soma e o bit de transporte são enviados aos pinos de saída `8` a `12`, prontos para serem utilizados por outros dispositivos ou circuitos.

5. **Execução Contínua**: O programa repete esses passos continuamente, aguardando um novo sinal no pino `13` para iniciar uma nova operação de soma.


# Contribuição

Para os contribuidores deste projeto, seu papel é essencial para melhorar e expandir o programa. Suas contribuições não apenas fortalecem o código existente, mas também enriquecem a comunidade Arduino, impactando positivamente o aprendizado e a inovação na tecnologia embarcada.
   


