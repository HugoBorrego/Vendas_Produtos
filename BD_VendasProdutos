-- Criação da tabela Produtos
CREATE TABLE Produtos (
    produtoID INT NOT NULL AUTO_INCREMENT COMMENT 'Identificação única do produto, incrementada automaticamente',
    nome VARCHAR(250) NOT NULL COMMENT 'Nome do produto',
    descricao VARCHAR(500) COMMENT 'Descrição do produto',
    categoria VARCHAR(150) COMMENT 'Categoria do produto',
    quantidade INT NOT NULL COMMENT 'Quantidade disponível do produto',
    preco DECIMAL(6,2) NOT NULL COMMENT 'Preço do produto com duas casas decimais',
    datavalidade DATE NOT NULL COMMENT 'Data de validade do produto',
    PRIMARY KEY (produtoID)
) DEFAULT CHARSET = utf8;

-- Criação da tabela Fornecedores
CREATE TABLE Fornecedores (
    fornecedorID int NOT NULL AUTO_INCREMENT COMMENT 'Identificação única do fornecedor, incrementada automaticamente',
    nome VARCHAR(250) NOT NULL COMMENT 'Nome do fornecedor',
    contato VARCHAR(12) NOT NULL COMMENT 'Contato do fornecedor',
    endereco VARCHAR(500) NOT NULL COMMENT 'Endereço do fornecedor',
    PRIMARY KEY (fornecedorID)
) DEFAULT CHARSET = utf8;

-- Criação da tabela Pedidos
CREATE TABLE Pedidos (
    pedidoID INT NOT NULL AUTO_INCREMENT COMMENT 'Identificação única do pedido, incrementada automaticamente',
    produtoID INT COMMENT 'Identificação do produto FK',
    fornecedorID INT COMMENT 'Identificação do fornecedor FK',
    datapedido DATE COMMENT 'Data do pedido',
    quantidade INT COMMENT 'Quantidade do pedido',
    status VARCHAR(500) NOT NULL COMMENT 'Status do pedido',
    PRIMARY KEY (pedidoID)
) DEFAULT CHARSET = utf8;

-- Criação da tabela Estoque
CREATE TABLE Estoque (
    produtoID INT COMMENT 'Identificação do produto FK',
    localID INT COMMENT 'Identificação do local de armazenamento FK',
    quantidade INT COMMENT 'Quantidade de produtos no estoque'
) DEFAULT CHARSET = utf8;

CREATE TABLE LocalArmazenamento (
    localID INT NOT NULL COMMENT 'Identificação única do local de armazenamento, incrementada automaticamente',
    nome VARCHAR(150) COMMENT 'Nome do local de armazenamento',
    descricao VARCHAR(500) COMMENT 'Descrição do local de armazenamento',
    PRIMARY KEY (localID)
) DEFAULT CHARSET = utf8;

-- Inserindo valores na tabela Produtos
INSERT INTO Produtos (nome, descricao, categoria, quantidade, preco, datavalidade) VALUES 
("Teclado", "Teclado mecânico com iluminação RGB", "Acessórios", 50, 129.99, '2026-12-31'),
("Mouse", "Mouse óptico sem fio", "Acessórios", 70, 89.99, '2026-11-30'),
("Monitor", "Monitor LED 24 polegadas", "Periféricos", 30, 999.99, '2026-10-15'),
("Notebook", "Notebook com processador i7 e 16GB RAM", "Computadores", 20, 4999.99, '2027-01-01'),
("HD Externo", "HD externo 1TB USB 3.0", "Armazenamento", 40, 299.99, '2026-09-25'),
("Impressora", "Impressora multifuncional a laser", "Periféricos", 15, 1499.99, '2026-08-20'),
("Fone de Ouvido", "Fone de ouvido Bluetooth com cancelamento de ruído", "Acessórios", 60, 199.99, '2026-07-15'),
("Placa de Vídeo", "Placa de vídeo GeForce RTX 3080", "Componentes", 10, 6999.99, '2026-06-10'),
("Fonte de Alimentação", "Fonte de alimentação 750W modular", "Componentes", 25, 349.99, '2026-05-05'),
("Teclado Gamer", "Teclado gamer com teclas programáveis", "Acessórios", 45, 259.99, '2026-04-01'),
("Mousepad", "Mousepad com superfície antiderrapante", "Acessórios", 80, 49.99, '2026-03-10'),
("Webcam", "Webcam full HD com microfone embutido", "Periféricos", 35, 299.99, '2026-02-15'),
("SSD", "SSD 512GB NVMe", "Armazenamento", 50, 799.99, '2026-01-20'),
("Memória RAM", "Memória RAM 8GB DDR4", "Componentes", 40, 399.99, '2026-12-05'),
("Gabinete", "Gabinete ATX com painel de vidro temperado", "Componentes", 20, 499.99, '2025-12-01'),
("Roteador", "Roteador Wi-Fi 6 dual band", "Redes", 25, 599.99, '2025-11-15'),
("Switch", "Switch de rede 8 portas Gigabit", "Redes", 30, 199.99, '2025-10-10'),
("Ventoinha", "Ventoinha para gabinete com iluminação LED", "Componentes", 60, 79.99, '2025-09-05'),
("Microfone", "Microfone condensador USB", "Acessórios", 50, 299.99, '2025-08-01'),
("Câmera de Segurança", "Câmera de segurança IP com visão noturna", "Segurança", 40, 399.99, '2025-07-01');

-- Inserindo valores na tabela Fornecedores
INSERT INTO Fornecedores (nome, contato, endereco) VALUES 
("Fornecedor A", "12912345678", "Endereço A"),
("Fornecedor B", "21345678901", "Endereço B"),
("Fornecedor C", "31345549753", "Endereço C");

-- Inserindo valores na tabela Pedidos
INSERT INTO Pedidos (datapedido, quantidade, status) VALUES 
('2025-06-01', 50, 'Concluído'),
('2025-06-10', 70, 'Pendente'),
('2025-06-15', 30, 'Concluído'),
('2025-06-20', 20, 'Pendente'),
('2025-07-01', 40, 'Concluído'),
('2025-07-10', 15, 'Pendente'),
('2025-07-15', 60, 'Concluído'),
('2025-07-20', 10, 'Pendente');

-- Inserindo valores na tabela LocalArmazenamento
INSERT INTO LocalArmazenamento (nome, descricao) VALUES 
("Armazém Central", "Local principal para armazenamento de produtos"),
("Depósito Secundário", "Local de armazenamento secundário para produtos excedentes");

-- Inserindo valores na tabela Estoque
INSERT INTO Estoque (quantidade) VALUES 
(25),
(35),
(15),
(10),
(20),
(5),
(30),
(5),
(12),
(25),
(40),
(17),
(30),
(20),
(8),
(12),
(15),
(30),
(40),
(10);
