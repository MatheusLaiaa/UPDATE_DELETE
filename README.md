# ATIVIDADE ANIMAL 

## METODOLOGIA

Essa atividade tem o intuito de trazer o aprendizado (DELETE, ALTER, UPDATE E DROP) de banco de dados, onde utilizamos o WorkBench MySql para poder desensolver de forma dinamica o exercicio proposto pelo nosso tutor. 

## PASSO A PASSO PEDIDO NO EXERCICIO

### Altere o nome do Pateta para Goofy;

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/e39f3738-afcc-43fd-9626-aecad9b94431)

UPDATE Animais
SET Nome = 'Goofy'
WHERE Nome = 'Pateta';


### Altere o peso do Garfield para 10 quilogramas;

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/d8ab6349-94a6-4612-a8f7-4dbb6eb27beb)

UPDATE Animais
SET Peso = 10
WHERE Nome = 'Garfield';


### Altere a cor de todos os gatos para laranja;

### Crie um campo altura para os animais;

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/4faaef18-001f-4479-bd0c-a6322b556c60)

ALTER TABLE Animais
ADD Altura DECIMAL(4, 1);


### Crie um campo observação para os animais;

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/82c14702-fd0c-48c5-b236-f42052596e62)

ALTER TABLE Animais
ADD Observacao TEXT;


### Remova todos os animais que pesam mais que 200 quilogramas.

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/011b75d2-fe45-4c1c-9477-58fded0e1a9e)

DELETE FROM Animais
WHERE Peso > 200;


### Remova todos os animais que o nome inicie com a letra ‘C’.

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/46a92527-15c4-45e6-8a7e-574e6f6f6cad)

DELETE FROM Animais
WHERE Nome LIKE 'C%';


### Remova o campo cor dos animais;

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/f653cd28-e7fb-4e5d-8f32-0a6166e70b66)

ALTER TABLE Animais
DROP COLUMN Cor;


### Aumente o tamanho do campo nome dos animais para 80 caracteres;

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/90514798-97df-4609-aaee-a70f95cda22c)

ALTER TABLE Animais
ALTER COLUMN Nome VARCHAR(80);


### Remova todos os gatos e cachorros.

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/a706f0c8-a0f3-41ae-9d60-19f91cbb7027)

DELETE FROM Animais
WHERE Nome IN ('Garfield', 'Frajola', 'Manda-chuva', 'Snowball', 'Gato de Botas', 'Kitty', 'Milu', 'Rex', 'Bidu', 'Dum Dum', 'Muttley', 'Scooby', 'Rufus');


### Remova o campo data de nascimento dos animais.

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/a73344c7-51ff-4e1e-acae-6f12960e68c7)

ALTER TABLE Animais
DROP COLUMN Data_Nascimento;


### Remova todos os animais.

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/541c65d1-d43c-437c-b040-9a1eace848c5)

DELETE FROM Animais;


### Remova a tabela especies.

![image](https://github.com/MatheusLaiaa/UPDATE_DELETE/assets/144149403/e9bfaa66-7b60-4e34-8594-cb6d13756c11)

DROP TABLE Animais;
















