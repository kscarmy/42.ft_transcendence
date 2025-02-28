# ft_transcendence

Le README reste a faire.

En attendant voici le .env \
Il est ignoré dans .gitignore, donc il faut bien le donner quelque part afin de tester le projet...\
Les secrets sont volontairement peut sécurisés, on devait pouvoir les utiliser facilement des dizaines de fois par heures. Si ce doit etre mis en prod, forcement que ce serait changé, et pas public sur github !

### Pour lancer le projet donc
```sh
touch .env
```

Inserer dedans les variables d'environnement suivantes :

```sh

# POSTGRES_HOST_AUTH_METHOD=trust
POSTGRES_USER=postgres             
POSTGRES_PASSWORD=postgres
POSTGRES_DB=postgres
POSTGRES_HOST=postgres
POSTGRES_PORT=5432
POSTGRES_ENGINE="django.db.backends.postgresql"

#grafana
GF_SECURITY_ADMIN_USER=grafana
GF_SECURITY_ADMIN_PASSWORD=adminpassword123
GF_SERVER_ROOT_URL=%(protocol)s://%(domain)s:%(http_port)s/grafana/
GF_SERVER_SERVE_FROM_SUB_PATH=true

# Discord alerts
DISCORD_WEBHOOK="https://discord.com/api/webhooks/1251195705301667872/KCoPeQygUtFXvGd-8g6_i7G16lnJ7414di6uaYVygTbgyBNSl4wyqdw8-zWNgGgqDwBQ"

# elasticsearch
ELASTIC_USERNAME=elastic
ELASTIC_PASSWORD=DidierDidier
bootstrap.memory_lock=true
discovery.type=single-node
xpack.security.enabled=true
xpack.monitoring.collection.enabled=true
xpack.security.http.ssl.enabled=false

# logstash
xpack.monitoring.enabled=true

# Blockchain settings
API_URL="https://eth-sepolia.g.alchemy.com/v2/4uryTCcwOBqa6dyrL9ajVJiTblBGXYgW"
PRIVATE_KEY="a5fd090aae2bfd9bf0b1bc3bef44dcbaaabc2681f891da32edbbfe5cc05ce5b5"
API_KEY="4uryTCcwOBqa6dyrL9ajVJiTblBGXYgW"
CONTRACT_ADDRESS="0x2971a35217A1c844C18aF535FbeC63d8A097760F"
ETHERSCAN_API_KEY="7KBZM4CKIPXNYN36BW1IC9BN94XA5R5D74"

# Django secret key
DJANGO_SECRET_KEY='ebL1UDQ:Dt2i2l2UvsJ3A@s=/t8[..:£2}",eRGg|7ie=^=M5u'

# SuperUser
SUPERUSER_ID='admin'
SUPERUSER_PASSWORD='02y5zTF#1{_~2['

```


Faites un 
```sh
make
```

Premier demarrage ? Docker va devoir telecharger et preparer un certain nombres d'images.\
Faites vous un café, revenez plus tard.

Bloqué ?

```sh
make help
```

### La documentation

dispo dans le dossier `./docs/`


## Auteurs

Projet réalisé par :
- [kscarmy](https://github.com/kscarmy)
- [MaloP47](https://github.com/MaloP47)
- [noapoleon](https://github.com/noapoleon)
- [ftrenstein](https://github.com/ftrenstein)
- [brunet-guillaume](https://github.com/brunet-guillaume)

