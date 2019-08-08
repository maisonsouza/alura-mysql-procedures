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

---

### Stored Procedures Básico

---

### Interações com o banco de dados.

---

### Controle de fluxo.

---

### Cursor e Função.

---

### Problema Prático.


