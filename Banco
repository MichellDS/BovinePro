CREATE TABLE agricultor (
    id INT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    senha VARCHAR(255) NOT NULL
);

CREATE TABLE raca (
    ID INT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL
);


CREATE TABLE fazenda (
    id INT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    area DECIMAL(10, 2) NOT null,
    agricultor_id INT,
    FOREIGN KEY (agricultor_id) REFERENCES agricultor(ID)
);


CREATE TABLE gado (
    id INT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    datanasc DATE NOT NULL,
    sexo CHAR(1) NOT NULL,
    raca_id INT,
    FOREIGN KEY (raca_id) REFERENCES Raca(ID),
    fazenda_id INT,
    FOREIGN KEY (fazenda_id) REFERENCES fazenda(ID)
);

CREATE TABLE producaoleite (
    id INT PRIMARY KEY,
    datatirada DATE NOT NULL,
    qtd INT NOT NULL,
    nome_id INT,
    FOREIGN KEY (nome_id) REFERENCES Gado(ID)
);
