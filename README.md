Projeto de Sistema Bancário
Este projeto é um sistema bancário simples implementado em Python. Ele permite a criação de clientes e contas, bem como a realização de transações como depósitos e saques. O sistema também permite a visualização do extrato de uma conta e a listagem de todas as contas criadas.

Funcionalidades
Criar Cliente: Cria um novo cliente no sistema.
Criar Conta: Cria uma nova conta corrente para um cliente existente.
Depositar: Realiza um depósito em uma conta do cliente.
Sacar: Realiza um saque de uma conta do cliente, respeitando limites de saque.
Exibir Extrato: Exibe o extrato das transações realizadas em uma conta do cliente.
Listar Contas: Lista todas as contas criadas no sistema.
Estrutura do Código
Classes Principais
Cliente: Representa um cliente do banco.

PessoaFisica: Representa um cliente pessoa física, derivado da classe Cliente.
Conta: Representa uma conta bancária.

ContaCorrente: Representa uma conta corrente, derivado da classe Conta.
Transacao (abstract): Classe abstrata para transações bancárias.

Saque: Representa uma transação de saque.
Deposito: Representa uma transação de depósito.
Historico: Armazena o histórico de transações de uma conta.

Funções Principais
menu(): Exibe o menu de opções para o usuário.
filtrar_cliente(cpf, clientes): Filtra e retorna um cliente pelo CPF.
recuperar_conta_cliente(cliente): Recupera a conta de um cliente.
depositar(clientes): Realiza um depósito em uma conta.
sacar(clientes): Realiza um saque de uma conta.
exibir_extrato(clientes): Exibe o extrato de uma conta.
criar_cliente(clientes): Cria um novo cliente.
criar_conta(numero_conta, clientes, contas): Cria uma nova conta para um cliente.
listar_contas(contas): Lista todas as contas criadas.
main(): Função principal que executa o loop do menu.
Como Executar
Certifique-se de ter o Python instalado na sua máquina.

Clone este repositório.

Navegue até o diretório do projeto.

Execute o script principal:

bash
Copiar código
python main.py
Exemplo de Uso
Ao iniciar o programa, você verá o seguinte menu:

css
Copiar código
================ MENU ================
[d]    Depositar
[s]    Sacar
[e]    Extrato
[nc]   Nova conta
[lc]   Listar contas
[nu]   Novo usuário
[q]    Sair
=> 
Escolha uma das opções digitando a letra correspondente e siga as instruções apresentadas.

Notas
Atualmente, o sistema não permite que um cliente escolha entre múltiplas contas. A função recuperar_conta_cliente sempre retorna a primeira conta do cliente.
O limite de saque e o número máximo de saques por dia são configuráveis na criação da conta corrente.
Melhorias Futuras
Permitir que o cliente escolha entre múltiplas contas.
Adicionar suporte para contas poupança e outras modalidades de contas.
Implementar autenticação de cliente.
Adicionar interface gráfica para facilitar o uso do sistema.
Licença
Este projeto é distribuído sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

Desfrute do seu sistema bancário simples em Python! Se tiver alguma dúvida ou sugestão, sinta-se à vontade para abrir uma issue ou um pull request.
