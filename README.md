# testePHP
Projeto criado para receber codificação em PHP para testes de conhecimentos.
# Especificações
Criar os CRUDs necessários para as seguintes estruturas de banco de dados (sugestão MySQL):
```
CREATE DATABASE teste;

CREATE TABLE pessoa (
	idPessoa INT NOT NULL AUTO_INCREMENT , 
	nome VARCHAR(200) NOT NULL , 
	dt_nascimento DATE NOT NULL , 
	escolaridade ENUM('Ensino Fundamental','Ensino Médio','Ensino Superior') NOT NULL , 
	PRIMARY KEY (idPessoa)
);

CREATE TABLE telefone(
    idTelefone INT NOT NULL AUTO_INCREMENT,
    idPessoa INT NOT NULL,
    telefone varchar(15),
    PRIMARY KEY (idTelefone),
    FOREIGN KEY (idPessoa) REFERENCES pessoa (idPessoa)
);
```
# Entendimento
O entendimento da estrutura e a maneira que a mesma será implementada faz parte do teste.
# Uso de bibliotecas
Permitido o uso de bibliotecas CSS e/ou JavaScript que desejar.
