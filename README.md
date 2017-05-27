# backupbdpostgres
Realizar o backup de um banco de dados postgres. 

#SHELLSCRIPTPARABACKUPBDPOSTGRE

#!/bin/sh

#bkp_livraria.sh

- #DATA iria imprimir a data: ano-mes-dia.

DATA='/bin/date+%Y-%m-%d'

- #NOME armazena o nome do arquivo de BACKUP

- #O Diretório onde o arquivo será salvo neste caso é:

#/www/virtual/backup é uma pasta publica do apache.

- #Coloque o diretorio onde quiser guardar o BACKUP.

NOME="/www/virtual/backup/livraria.sh-$DATA.sql"

- #Variaveis do POSTGRESQL

HOST="localhost"

USER="postgres"

PASSWORD="12345"

DATABASE="livraria.sh"

pg_dump -h $localhost -u $postgres -p $12345 $livraria.sh > $livraria.backup
