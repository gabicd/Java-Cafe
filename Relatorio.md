# Java Café
**Grupo:**  _Emilie Nelise Rodrigues da Silva  (12557546) / Gabriela Carvalho Dantas (14572832) / Pedro Eduardo Moreira Chamone (14675823)_

## Requisitos
### Interface de usuário
- Projete uma GUI simples e intuitiva usando JavaFX.
- A interface deve incluir botões para adicionar itens a um pedido, concluir transações e visualizar relatórios de estoque e vendas.
### Processamento de pedido
- Permita que os usuários criem novos pedidos, adicionem itens do menu e finalizem vendas.
- Cada pedido deve calcular o custo total, aplicar impostos e gerar um recibo.
### Gestão de inventário
- Implemente um sistema para rastrear os níveis de estoque de produtos.
- Atualize o estoque automaticamente quando os pedidos forem processados.
- Alerte os usuários quando os níveis de estoque estiverem baixos.
### Manipulação de exceção:
- Tratamento robusto de erros para entradas do usuário, gerenciamento de inventário e operações de arquivo.
- Implemente exceções personalizadas para cenários de erro específicos, como "Esgotado" ou "Tipo de pagamento inválido".
### Armazenamento de dados
- Use I/O de arquivo para armazenar e recuperar dados de estoque e registros de vendas.
- Garanta a persistência dos dados entre sessões salvando as alterações em um arquivo.
### Documentação
Documente minuciosamente o código, concentrando-se especialmente em métodos públicos e interfaces de usuário.
Forneça um manual do usuário que explique como operar o sistema POS.
## Descrição do Projeto
O sistema java café, trata-se de um sistema 'Point of Sales' de um pequeno café. O sistema deve conter uma página com os itens, em que o usuário pode efetuar uma compra, adicionando ou diminuindo a quantidade de itens. Ao finalizar a compra, geramos um recibo e automaticamente a compra fica em nosso histórico de vendas. Também devemos conseguir editar o estoque e limitar a quantidade de pedidos via estoque. 
## Comentários sobre o código
Um breve resumo de cada classe:
- *MainFrame:* Responsável pela implementação da janela principal da nossa interface. Contém a função main();
- *FileController:*  Gerencia operações relacionadas a arquivos, como leitura, escrita e manipulação de dados em arquivos do sistema.

- *LoginController:* Controla o processo de autenticação de usuários, incluindo verificação de credenciais e gerenciamento de sessões de login.

- *InventoryController:* Administra o inventário do sistema, incluindo adição, remoção e atualização de itens no estoque.

- *InventoryPageController:* Gerencia a interface de usuário relacionada à página de inventário, facilitando a interação entre o usuário e os dados de inventário.

- *mainPageController:*  Controla a navegação e as operações na página principal da aplicação, servindo como ponto central de controle.

- *orderController:* Gerencia a criação, atualização e rastreamento de pedidos dentro do sistema, incluindo processamento de compras e vendas.

- *PageNavigationController:* Facilita a navegação entre diferentes páginas e seções da aplicação, assegurando uma experiência de usuário fluida.

- *salesController:* Controla operações relacionadas a vendas, incluindo processamento de transações e geração de relatórios de vendas.

- *Inventory:* Representa o inventário em si, incluindo dados sobre os itens estocados e suas quantidades.

- *User:* Modela um usuário do sistema, incluindo informações pessoais, credenciais de login e permissões de acesso.

- *newUserController:* Gerencia o processo de criação de novos usuários, incluindo coleta de informações e configuração inicial de contas.

- *Scene1controller:*  Controla a lógica e a interação da primeira cena ou tela da aplicação, configurando o ambiente inicial para o usuário.


## Plano e Resultado de Testes 
### Projeção da Interface de Usuário (GUI)
#### Plano
  - Projetar uma GUI simples e intuitiva usando JavaFX.
  - Incluir botões para adicionar itens a um pedido, concluir transações e visualizar relatórios de estoque e vendas.
#### Teste 
  - Verificar se a interface é intuitiva e responsiva.
  - Testar cada botão para garantir que ele realiza a ação correta (adicionar itens, concluir transações, visualizar relatórios).

###Processamento de Pedido
#### Plano
- Permitir que os usuários criem novos pedidos, adicionem itens do menu e finalizem vendas.
- Cada pedido deve calcular o custo total, aplicar impostos e gerar um recibo.
#### Teste
- Criar vários pedidos de teste para verificar se o cálculo do custo total e a aplicação de impostos estão corretos.
- Validar se o recibo gerado contém todas as informações necessárias e corretas.
- Testar a adição e remoção de itens em um pedido para garantir que as quantidades e os preços são atualizados corretamente.

### Gestão de Inventário
#### Plano
- Implementar um sistema para rastrear os níveis de estoque de produtos.
- Atualizar o estoque automaticamente quando os pedidos forem processados.
- Alertar os usuários quando os níveis de estoque estiverem baixos.
### Teste
- Simular a criação e processamento de pedidos para verificar se o estoque é atualizado corretamente.
- Testar o alerta de estoque baixo criando pedidos que diminuam o estoque para níveis críticos.
- Verificar se o sistema impede pedidos de itens esgotados.

### Manipulação de Exceção
#### Plano
- Implementar tratamento robusto de erros para entradas do usuário, gerenciamento de inventário e operações de arquivo.
- Implementar exceções personalizadas para cenários de erro específicos, como "Esgotado" ou "Tipo de pagamento inválido".
#### Teste
- Testar entradas inválidas do usuário (e.g., quantidade negativa, caracteres não numéricos em campos numéricos) para garantir que o sistema lida corretamente com esses erros.
- Simular erros de inventário, como tentar processar um pedido com itens esgotados, e verificar se as exceções personalizadas são acionadas corretamente.
- Testar falhas em operações de arquivo, como tentar salvar dados em um local de armazenamento não acessível, para garantir que o sistema lida com esses erros de forma robusta.

### Armazenamento de Dados
#### Plano
- Usar I/O de arquivo para armazenar e recuperar dados de estoque e registros de vendas.
- Garantir a persistência dos dados entre sessões salvando as alterações em um arquivo.
#### Teste
- Verificar se os dados de estoque e vendas são corretamente salvos em arquivos após cada operação relevante.
- Testar a recuperação de dados ao iniciar o sistema para garantir que os dados persistentes são carregados corretamente.
- Simular interrupções (e.g., fechamento inesperado do sistema) para garantir que os dados ainda são consistentes após a reinicialização.

### Documentação
#### Plano
- Documentar minuciosamente o código, concentrando-se especialmente em métodos públicos e interfaces de usuário.
- Fornecer um manual do usuário que explique como operar o sistema POS.
#### Teste
- Revisar a documentação do código para garantir que todos os métodos e interfaces estão adequadamente documentados.
- Testar o manual do usuário com usuários não familiarizados com o sistema para garantir que ele é claro e completo.

## Descrição do Projeto
### Sistema Java Café
O sistema Java Café é um sistema "Point of Sales" (POS) para um pequeno café. O sistema deve conter uma página com os itens disponíveis, onde o usuário pode efetuar compras adicionando ou diminuindo a quantidade de itens. Ao finalizar a compra, um recibo é gerado e a compra é registrada no histórico de vendas. O sistema também deve permitir a edição do estoque e limitar a quantidade de pedidos com base no estoque disponível.

## Procedimentos de Construção
### Comandos para Executar o Programa
- Para a execução, usamos a IDE IntelliJ

1. Baixar a biblioteca JavaFx
2. Configurar a  @biblioteca
2.1.  Clicar nessa barrinhar > Ir em Project Structure > Adicionar a lib do JavaFx em Global Libraries
![funciona](https://github.com/emilie-nelise/Java-Caf-/assets/105816701/03b92a5f-c134-4962-8354-437f4e2ff741)
![teste](https://github.com/emilie-nelise/Java-Caf-/assets/105816701/f24af778-a34f-434e-9df3-f0a88e12125c)
2.2 Na mesma tela (Project Structure) > Adicionar em Modules a lib do JavaFx 
![teste2](https://github.com/emilie-nelise/Java-Caf-/assets/105816701/d4f843ce-aad3-482b-ac17-e2c340888502)
2.3 Agora, em Run > Edit Configurations
![tites](https://github.com/emilie-nelise/Java-Caf-/assets/105816701/64c97916-7154-48fe-aaac-c6093ce0948a)
- Clique em Modify Options > Add VM Options
- Coloque a opção de java 22, no local marcado da imagem
- Na linha abaixo, copie e cole o seguinte caminho:
*--module-path "C:\Users\gabis\Desktop\javafx-sdk-22.0.1\lib" --add-modules javafx.controls,javafx.fxml*
Mas, na parte entre parênteses, troque pelo caminho até a lib do javafx da sua máquina. 
- Após isso, no campo vazio abaixo, escreva javacafe.Main
- Pode rodar!

## Problemas durante o Projeto

- De início, tivemos dificuldade na configuração do JavaFX para começar a construção do projeto.
- Outra dificuldade, foi na organização dos updates do nosso código. Dividimos nossas partes e trabalhamos separadamente, cada um fazendo updates no git hub, mas em seu próprio código. Isso dificultou o andamento do projeto, pois no fim, tivemos retrabalho e precisamos juntar cada parte separadamente. 
- Tivemos problemas com a edição da configuração de estoque, não conseguindo entregá-la.


