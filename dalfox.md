dalfox url http://testphp.vulnweb.com/artists.php?artist=1

katana -u http://testphp.vulnweb.com/ | gf xss | tee -a xss.txt

cat xss.txt | dolfox pipe

dalfox file xss.txt

