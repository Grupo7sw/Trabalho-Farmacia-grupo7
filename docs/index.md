<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
*&lt;Sistema de Gestão para a Farmácia Vida Saudável&gt;*
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do Projeto](#introdução-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#descrição-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-comportamento-atores)
- [Descrição dos Casos de Uso](#descrição-das-funcões)
- [Diagrama de Senquencia](#diagrama-de-ordem-interações)
- [Diagrama de Classes](#diagrama-orientado-objetos)
- [Diagrama de Estados](#diagrama-estrutura-componente)
- [Diagrama de Implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* CAIO YUKIO YAZAWA - 10418604
* GABRIEL FREITAS DE MIRANDA CORREA - 10425934 
* GIOVANE ZERBINATO DE JESUS - 10417013 

# Descrição do Projeto

A Farmácia Vida Saudável busca modernizar sua gestão com um sistema informatizado para otimizar vendas, estoque e atendimento, garantindo mais eficiência e precisão.

# Análise de Requisitos Funcionais e Não-Funcionais
**Requisitos Funcionais:**

1. **Cadastro de Produtos e Medicamentos**
   O sistema deve permitir o cadastro de medicamentos e produtos com nome, descrição, fabricante, lote, data de validade e quantidade em estoque. O sistema também deve permitir a inserção e atualização do preço de venda de cada produto.
   
2. **Cadastro de Clientes**
   O sistema deve permitir o cadastro de clientes com nome, CPF e telefone, armazenando o histórico de compra de cada cliente.
   
3. **Processo de Venda**
   O sistema deve permitir a visualização dos produtos em estoque e o registro de vendas vinculadas a clientes. Depois de finalizar uma venda, o sistema emitirá automaticamente um cupom fiscal e atualizará o inventário, assegurando que as informações estejam constantemente atualizadas.
   
4. **Controle de Estoque**
   O sistema deve manter a quantidade de produtos no estoque atualizada após cada venda e emitir alertas para itens com estoque baixo.
   
5. **Relatórios Gerenciais**
   O sistema deve gerar relatórios de vendas diárias, semanais e mensais, o sistema também deve gerar relatório dos produtos mais vendidos e dos clientes mais frequentes.
   
6. **Autenticação e Controle de Acesso**
   O sistema deve permitir a criação de perfis de atendente e administrador, onde os atendentes podem realizar vendas e consulta de estoque, e os administradores podem cadastrar produtos, gerar relatórios e visualizar o histórico completo.
   
**Requisitos Não Funcionais:**

1. **Desempenho**
   O sistema deve responder às consultas de produtos e processar vendas no menor tempo possível
   
2. **Segurança**
   O sistema deve exigir autenticação para acessar funções administrativas.
   
   O sistema deve registrar todos os acessos realizados
   
   O sistema deve garantir que os dados de usuário sejam armazenados de forma segura com criptografia.
   
   O sistema deve estar sempre atualizado na versão mais recente.
   
4. **Disponibilidade**
    O sistema deve estar disponível durante todo o período comercial e realizar backup periódico para salvar dados e informações.
   
5. **Redimensionamento**
    O sistema precisa ser capaz de expandir a base de dados sem comprometer o desempenho.
    O sistema deve possibilitar a inclusão de novos produtos e usuários sem precisar de um reajuste. 

# Diagrama de Atividades

![DiagramaATV](https://github.com/user-attachments/assets/20e9c4cc-ceea-46ff-a480-90a12a107df0)


# Diagrama de Casos de Uso

![image](https://github.com/user-attachments/assets/d03bd69b-0fa1-4104-a047-232d9e99787d)


# Descrição dos Casos de Uso

**Atores**

1. Usuário (generalização)

Representa um ator genérico do sistema, podendo ser um Admin, Cliente ou Gerente.

2. Admin

Responsável por gerenciar aspectos administrativos e de segurança do sistema.

3. Cliente
   
Usuário final que realiza compras no sistema.

4. Gerente
   
Responsável por atividades operacionais e gerenciais, como cadastro de produtos, gestão de clientes e vendas.

**Casos de uso**

**Admin**

**Autenticação e controle de acesso:**

   Permite ao Admin gerenciar o login e as permissões de usuários no sistema.

**Cliente**

**Registrar compras:**

   O cliente pode registrar suas compras no sistema.

   <<include>> Atualizar estoque: Cada compra registrada resulta na atualização automática do estoque.

**Gerente**

**-Cadastrar produtos e medicamentos**

   Permite ao gerente inserir novos produtos ou medicamentos no sistema.

**-Gerenciar clientes**

   Possibilita ao gerente alterar ou atualizar informações dos clientes.

**-Registrar vendas**

   O gerente pode registrar vendas realizadas.

   <<extend>> Emitir nota fiscal: Opcionalmente, o sistema pode emitir uma nota fiscal ao registrar uma venda.

   <<include>> Atualizar estoque: A venda resulta na atualização do estoque.

**-Gerar Relatórios**

   Possibilita ao Admin extrair dados do sistema em formato de relatórios para análise.

# Diagrama de Sequência

![Diagrama de Sequência drawio](https://github.com/user-attachments/assets/dcec6632-e37c-4d88-8b4d-841d63376a89)

# Diagrama de Classes

![diagrama classe](https://github.com/user-attachments/assets/1d3cf075-9ec9-48cb-9aa3-dc54b06ac975)


# Diagrama de Estados

![image](https://github.com/user-attachments/assets/86430626-42ef-43f4-b452-3a86cfd34a44)


# Diagrama de Implantação

![diagrama - implementação](https://github.com/user-attachments/assets/fc449ff9-09b6-4a9f-8b48-1dd56868e66a)



# Referências

OWASP - https://owasp.org/Top10/pt_BR/

Lucidchart - https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml

Material complementar visto em sala
