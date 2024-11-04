Sistema de Gerenciamento de Produtos - CRUD em Java

Descrição:
Este é um sistema de gerenciamento de produtos implementado em Java Puro, que permite ao usuário realizar operações CRUD (Criar, Ler, Atualizar e Deletar) em produtos, além de funcionalidades de busca por ID, nome e categoria. O sistema é estruturado para rodar em ambiente de console.

Estrutura do Projeto

com.loja/
├── modelo/            # Classes de modelo/entidades

│   └── Produto.java   # Classe que representa o produto

├── gerenciador/       # Classes de gerenciamento de dados

│   └── GerenciadorProdutos.java   # Gerencia as operações de CRUD e busca

├── ui/                # Interface de usuário (console)

│   └── MenuProdutos.java          # Exibe o menu de interação com o usuário

├── exception/         # Exceções personalizadas

│   ├── ProdutoException.java      # Exceção geral para produtos

│   └── ValidacaoException.java    # Exceção para validação de dados

└── Main.java          # Classe principal para iniciar o sistema

Funcionalidades

Cadastrar Produto:
Solicita nome, preço, quantidade em estoque e categoria.
Valida as entradas e adiciona o produto ao sistema.

Buscar Produto por ID:
Pesquisa o produto pelo ID e exibe suas informações.

Listar Todos os Produtos:
Exibe a lista completa de produtos cadastrados.

Atualizar Produto:
Permite editar as informações de um produto existente após uma busca pelo ID.

Deletar Produto:
Remove o produto com o ID especificado.

Buscar por Nome:
Exibe todos os produtos que contêm o nome especificado (busca insensível a maiúsculas/minúsculas).

Buscar por Categoria:
Exibe produtos da categoria especificada.

Exceções Personalizadas:
ProdutoException: Para tratar erros gerais relacionados a produtos.
ValidacaoException: Para tratar erros de validação (e.g., nome vazio, preço negativo).

Exemplos de Uso:

===== Sistema de Gerenciamento de Produtos =====
1. Cadastrar Produto
2. Buscar Produto por ID
3. Listar Todos os Produtos
4. Atualizar Produto
5. Deletar Produto
6. Buscar por Nome
7. Buscar por Categoria
8. Sair
Escolha uma opção:

Criação de Produto

 === Cadastro de Produto ===
 Digite o nome: Notebook
 Digite o preço: 2500.00
 Digite a quantidade: 10
 Digite a categoria: Eletrônicos
 Produto cadastrado com sucesso!
 ID gerado: 1

 Busca de Produto

 === Busca de Produto ===
 Digite o ID: 1
 Produto encontrado:
ID: 1 | Nome: Notebook | Preço: R$ 2500,00 | Estoque: 10 | 
Categoria: Eletrônicos

Requisitos
Java: Versão 17 ou superior.

Como Executar
Clone o repositório:
git clone https://github.com/Tulio369/gerenciamento-produtos.git

Compile o projeto:
javac -d bin src/com/loja/*.java src/com/loja/*/*.java

Execute o programa:
java -cp bin com.loja.Main

Contribuição
Para contribuir com o projeto:
Faça um fork do repositório.

Crie uma branch para sua funcionalidade:
git checkout -b feature/nome-da-funcionalidade

Faça um commit das suas alterações:
git commit -m "Descrição da funcionalidade"

Envie suas alterações para o repositório:
git push origin feature/nome-da-funcionalidade
Abra um Pull Request.

Licença
Esse projeto está licenciado sob a MIT License.
