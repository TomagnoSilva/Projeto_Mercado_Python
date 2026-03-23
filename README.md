# Mercado Python

## Descrição
Este é um sistema simples de mercado desenvolvido em Python, utilizando programação orientada a objetos. O projeto permite cadastrar produtos, listar produtos disponíveis, adicionar produtos ao carrinho, visualizar o carrinho e fechar pedidos.

## Funcionalidades
- **Cadastrar Produto**: Permite adicionar novos produtos ao sistema com nome e preço.
- **Listar Produtos**: Exibe todos os produtos cadastrados com seus códigos, nomes e preços.
- **Comprar Produto**: Permite adicionar produtos ao carrinho informando o código do produto.
- **Visualizar Carrinho**: Mostra os produtos adicionados ao carrinho com suas quantidades.
- **Fechar Pedido**: Calcula o valor total da compra, exibe a fatura e limpa o carrinho.
- **Sair do Sistema**: Encerra o programa.

## Pré-requisitos
- Python 3.6 ou superior instalado no sistema.
- Recomenda-se o uso de um ambiente virtual (venv) para isolamento de dependências.

## Instalação
1. Clone ou baixe o repositório para o seu diretório local.
2. Navegue até o diretório do projeto:
   ```
   cd c:\Users\FartechGamer\Desktop\Projeto_Mercado_Python
   ```
3. (Opcional) Crie e ative um ambiente virtual:
   ```
   python -m venv venv
   venv\Scripts\activate  # No Windows
   ```
4. Não há dependências externas; o projeto utiliza apenas a biblioteca padrão do Python.

## Como Executar
1. Certifique-se de que o Python 3.x está instalado.
2. Navegue até o diretório do projeto: `cd c:\Users\FartechGamer\Desktop\Projeto_Mercado_Python`
3. Execute o arquivo principal: `python mercado.py`
4. Siga as instruções no menu interativo.

## Como Usar
Após executar o programa, você verá um menu com as seguintes opções. Digite o número correspondente e pressione Enter para selecionar uma ação. Aqui está um guia passo a passo:

### 1. Cadastrar Produto
- Selecione a opção 1.
- Digite o nome do produto (exemplo: "Maçã").
- Digite o preço do produto (exemplo: 5.50).
- O produto será cadastrado e você retornará ao menu principal.

### 2. Listar Produtos
- Selecione a opção 2.
- Se houver produtos cadastrados, eles serão exibidos um por um com código, nome e preço.
- Se não houver produtos, uma mensagem informará isso.
- Após a listagem, você retornará ao menu.

### 3. Comprar Produto
- Selecione a opção 3.
- Se houver produtos, eles serão listados.
- Digite o código do produto desejado (exemplo: 1).
- O produto será adicionado ao carrinho. Se já estiver no carrinho, a quantidade será incrementada.
- Você retornará ao menu.

### 4. Visualizar Carrinho
- Selecione a opção 4.
- Se houver itens no carrinho, eles serão exibidos com nome e quantidade.
- Se o carrinho estiver vazio, uma mensagem informará isso.
- Você retornará ao menu.

### 5. Fechar Pedido
- Selecione a opção 5.
- Se houver itens no carrinho, eles serão listados com quantidades e o valor total será calculado e exibido.
- O carrinho será esvaziado após o fechamento.
- Você retornará ao menu.

### 6. Sair do Sistema
- Selecione a opção 6.
- O programa será encerrado com uma mensagem de despedida.

**Nota**: Se você digitar uma opção inválida, o programa informará e retornará ao menu.

## Estrutura do Projeto
```
Projeto_Mercado_Python/
├── mercado.py          # Arquivo principal com o menu e lógica do sistema
├── teste.py            # Arquivo de teste para validação das funcionalidades
├── models/
│   ├── __init__.py     # Inicializa o módulo models
│   ├── produto.py      # Classe Produto: define atributos e métodos para produtos
│   └── __pycache__/    # Cache de bytecode gerado automaticamente
└── utils/
    ├── __init__.py     # Inicializa o módulo utils
    ├── helper.py       # Funções auxiliares, como formatação de moeda
    └── __pycache__/    # Cache de bytecode gerado automaticamente
```

## Arquitetura e Design
O projeto segue os princípios da programação orientada a objetos:
- **Classe Produto**: Encapsula os dados de um produto (código, nome, preço) e fornece métodos para manipulação.
- **Módulo utils**: Contém funções utilitárias reutilizáveis, como formatação de valores monetários.
- **Arquivo Principal (mercado.py)**: Gerencia o fluxo do programa, interações com o usuário e coordenação entre classes.

## Testes
Para executar os testes:
1. Execute o arquivo `teste.py`:
   ```
   python teste.py
   ```
2. Este arquivo contém testes básicos para validar as funcionalidades do sistema.

## Desenvolvimento
- **Contribuição**: Sinta-se à vontade para contribuir com melhorias, correções de bugs ou novas funcionalidades. Abra uma issue ou envie um pull request.
- **Diretrizes**: Mantenha o código limpo, adicione comentários onde necessário e siga as convenções de nomenclatura do Python (PEP 8).
- **Versionamento**: Use Git para controle de versão.

## Licença
Este projeto é de código aberto e está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.