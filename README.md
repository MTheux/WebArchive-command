Command

Filtro para OSINT 

curl -s https://crt.sh/?q=%.tesla.com&output=json | jq -r '.name_value' | grep -Po '{\\w+,\\w+,\\w+}*' > certsh.txt

http://web.archive.org/cdx/search/cdx?url=*.url.com.br/*&output=txt&fl=original 
