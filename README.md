## Descrição do Projeto
O sistema Java Café é um POS para um pequeno café. Ele permite que os usuários realizem compras, gerem recibos, mantenham histórico de vendas e gerenciem o estoque.

## Requisitos
### Interface de Usuário
- GUI intuitiva com JavaFX.
- Botões para adicionar itens, concluir transações e visualizar relatórios.

### Processamento de Pedido
- Criação de pedidos, cálculo de custo, aplicação de impostos e geração de recibos.

### Gestão de Inventário
- Rastreamento de estoque, atualização automática e alertas para níveis baixos.

### Manipulação de Exceção
- Tratamento robusto de erros e exceções personalizadas.

### Armazenamento de Dados
- Persistência de dados de estoque e vendas usando I/O de arquivo.

## Estrutura do Código
- **MainFrame:** Janela principal.
- **FileController:** Operações de arquivo.
- **LoginController:** Autenticação de usuários.
- **InventoryController:** Gestão de inventário.
- **InventoryPageController:** Interface de inventário.
- **mainPageController:** Página principal.
- **orderController:** Gerenciamento de pedidos.
- **PageNavigationController:** Navegação entre páginas.
- **salesController:** Operações de vendas.
- **Inventory:** Modelo de inventário.
- **User:** Modelo de usuário.
- **newUserController:** Criação de novos usuários.
- **Scene1controller:** Controle da primeira cena.

## Testes
- **GUI:** Testar usabilidade e funcionalidade dos botões.
- **Pedidos:** Verificar cálculos e geração de recibos.
- **Inventário:** Testar atualização e alertas de estoque.
- **Exceções:** Validar tratamento de entradas inválidas e erros.
- **Dados:** Testar salvamento e recuperação de dados.

## Execução do Programa
1. Baixar as bibliotecas JavaFX e JFoenix.
2. Adicionar as bibliotecas na IDE.
3. Configurar em Project Structure e Modules.
4. Em Run > Edit Configurations, adicionar VM Options:
--module-path "C:\caminho\para\javafx-sdk-22.0.1\lib" --add-modules javafx.controls,javafx.fxml
5. Configurar entrada principal como `javacafe.Main`.
6. Baixar a fonte https://www.dafont.com/superstar-2.font para visualização do programa na fonte idealizada para interface

## Problemas durante o Projeto
- Configuração inicial do JavaFX.
- Organização de updates de código no GitHub.
- Dificuldades na edição do estoque.
