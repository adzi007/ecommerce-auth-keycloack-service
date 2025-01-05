# Export keycloack Config

**Enter container terminal**
``
docker exec -it 3bc66deadfe9 /bin/bash
``

**Move to /opt/keycloak/bin/**

```
cd /opt/keycloak/bin/
```

**Export Config**
```
./kc.sh export --file /tmp/keycloak.json

or 

./kc.sh export --file keycloak.json
```

**Copy from container to host directory**

```
docker cp 3bc66deadfe9:/tmp/keycloak.json ./keycloack/
```

fixing failed import data:
https://medium.com/@ramanamuttana/script-upload-is-disabled-in-keycloak-4cb22d9358c8
https://howtodoinjava.com/devops/keycloak-script-upload-is-disabled/



