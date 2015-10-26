antonio
=======
curl -s http://sgp.postcodebase.com/node/[1-124289] | awk -F '<|>''
/itemprop=.description/ { printf "%s\031", $3 }
/itemprop=.postalCode/  { printf "%s\030", $7 }' >> "/tmp/postcodes.asv"
Repository of Antonio Tony
