# Export sql schema from commandline:
  mysqldump --add-drop-table -u admin -p`cat /etc/psa/.psa.shadow` dbname > dbname.sql
