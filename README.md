# dockerSymfony5
docker compose for symfony 5

# come usare questo docker compose

- avviare la procedura cone docker-compose up
- sulla porta 8000 potrete vedere symfony5 in esecuzione
- per settare il database mysql per symfony5 fare cosi:
  andare dentro al file .env
  
  DATABASE_URL=mysql://db_user:db_pass@mysql:3306/nomedb?serverVersion=5.7
  
  dove c'è mysql sarebbe lo spazio dedicato all'indirizzo dell'host, quindi ci si mette il nome del container che gestisce il 
  servizio di mysql.

  Poi bisogna andare nella root del container di symfony , all'interno della cartella di myapp e lanciare il comnado
  
  php bin/console doctrine:database:create
  
  (comando che genara il db)
  
