# Anotações do Curso de  Procedures SQL: Executando código no MySQL
![](https://www.alura.com.br/assets/api/share/curso-mysql-procedures.png)
## [Link do curso](https://cursos.alura.com.br/course/mysql-procedures)

### Preparando o ambiente
#### Visão geral do curso
> Instalação no Windows.

* Instalação do Mysql Installer.
* IDE Mysql Workbench.
* Developer Default.

> Instalação no Ubuntu
* Comando para verificar se o Mysql está instalado
```
dpkg -l mysql-server
mysql -V
```
* Comando para remover o Mysql
```
sudo apt-get remove --purge mysql*
sudo apt-get purge mysql*
sudo apt-get autoremove
sudo apt-get autoclean
```
* Comando para instalar o Mysql
```
sudo apt-get install mysql-server
sudo apt-get install mysql-workbench
```
* Configurando o Mysql
```
sudo mysql_secure_installation
Se você quiser fazer login como root através de programas externos:
sudo mysql -u root
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'senha_da_nasa';
```
##### Recuperando a base de dados
* Para realizar o curso deve ser feito a recuperação da base de dados no workbench.

---

### Stored Procedures Básico
* O sql não possui uma linguagem de programação estruturada que permita realizar comandos de programação(decisão, repetição)
DELIMITER (Separador de linha)

#### Exemplo de Stored Procedure
```
CREATE DEFINER=`root`@`localhost` PROCEDURE `sp_com_comentarios`()
BEGIN
/* Vamos exibir itens combinados entre textos e números */
-- Usando a função CONCAT
SELECT concat('Alô Mundo!!!', '......',(1+9)-5) as itens_combinados_com_comentarios;
END
```

#### Para chamar a Stored Procedure
```
call nome_da_stored_procedure;
```

#### Para alterar um Stored Procedure
```
USE `sucos_vendas`;
DROP procedure IF EXISTS `mostra_numero`;
```
Não há um comando para alterar, devemos excluir e criar novamente.

#### Declarando variáveis
```
declare ts datetime default localtimestamp();

```

---

### Interações com o banco de dados.

---

### Controle de fluxo.

---

### Cursor e Função.

---

### Problema Prático.


