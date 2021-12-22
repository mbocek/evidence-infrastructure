# evidence-infrastructure

Create .env file with content:
```
LOCAL_DOMAIN=evidence.lan
DEFAULT_NETWORK=evidence_net
DB_EVIDENCE_PWD=evidence
DB_EVIDENCE_DATA=/var/lib/postgresql/evidence/data
```
Run commands for initialisation of the environment:
```
docker network create evidence_net
docker-compose up
```
Edit hosts file (windows: %WinDir%\System32\Drivers\Etc\hosts
) add:
```
127.0.0.1 ui.evidence.lan
```

