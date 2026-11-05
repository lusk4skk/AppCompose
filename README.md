1. O que é entrada em um sistema computacional? Dê dois exemplos.
- Entrada é toda informação fornecida ao sistema, podendo vir de uma pessoa, arquivo, sensor, banco de dados ou outro sistema. Dois exemplos citados no contexto da aplicação são o preço do produto e o percentual de desconto informados pelo usuário.   

2. Qual é a diferença entre processamento e saída?
- Processamento é o conjunto de operações executadas sobre os dados de entrada (como calcular o desconto e subtrair do valor original), enquanto saída é a informação produzida por esse processamento e apresentada ao sistema (como o preço final com desconto).   

3. Por que o valor digitado em um TextField é inicialmente tratado como texto?
- Porque o componente TextField trabalha intrinsecamente com texto (String), exigindo uma conversão explícita para tipos numéricos (como Double) quando vamos realizar operações matemáticas.   

4. Qual é a finalidade de remember e mutableStateOf?
- mutableStateOf cria um estado observável pelo Compose, sinalizando que a interface precisa ser atualizada quando seu valor muda, e remember mantém esse valor armazenado durante as recomposições da função Composable, impedindo que seja reinicializado a cada execução.   

5. O que é um evento? Cite os eventos utilizados nesta aplicação.
- Evento é algo que acontece durante a interação do usuário com a aplicação, como digitar ou tocar em um botão. Os eventos utilizados são o onValueChange (para capturar as alterações no TextField) e o onClick (para responder ao toque no Button).   

6. O que significa recomposição no Jetpack Compose?
- Recomposição é o processo em que o Compose reexecuta as funções Composable necessárias para refletir mudanças de estado na tela, sem precisar reconstruir o aplicativo inteiro do zero.   

7. Qual é a responsabilidade da MainActivity neste projeto?
- É o ponto de entrada da aplicação Android, responsável por iniciar o conteúdo Compose através do bloco setContent e chamar a função de tela principal (CalculadoraDescontoScreen).   

8. Qual é a responsabilidade de CalculadoraDescontoScreen?
- Agrupar os componentes visuais, manter os estados necessários, capturar os eventos de interação, coordenar a chamada à regra de negócio e apresentar o resultado final ao usuário.   

9. Por que calcularPrecoComDesconto foi colocada em outro arquivo?
- Para separar as responsabilidades de forma lógica e limpa, isolando a regra matemática/de negócio da interface de usuário e da camada visual baseada em Compose.   

10. Qual é a vantagem de uma função de regra de negócio não depender do Compose?
- Isso torna a regra independente do framework Android e da interface gráfica, facilitando a manutenção, a reutilização do código e a realização de testes unitários sem misturar lógica de cálculo com layout visual.
