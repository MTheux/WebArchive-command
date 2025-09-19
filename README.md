Command

Filtro para OSINT 

curl -s https://crt.sh/?q=%.tesla.com&output=json | jq -r '.name_value' | grep -Po '{\\w+,\\w+,\\w+}*' > certsh.txt
curl -s "https://crt.sh/?q=%.url.com.br&output=json" | jq -r '.[].name_value' | sed 's/\*\.//g' | sort -u

http://web.archive.org/cdx/search/cdx?url=*.url.com.br/*&output=txt&fl=original 
