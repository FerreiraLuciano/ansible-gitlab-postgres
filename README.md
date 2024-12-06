# Luciano FERREIRA devops - Ansible Gitlab Postgres

## Configuration

Dans les fichiers "inventory.yml" et "/roles/gitlab/vars/main.yml" ne pas oublier de modifier l'addresse ip de la machine cible
``<192.168.66.10>``

## Commandes

### Déployer avec Docker

```bash
    docker-compose -f docker/docker-compose.yml build
    
    docker-compose -f docker/docker-compose.yml up -d
```

### Déployer avec ansible

```bash
  ansible-playbook -i inventory.yml playbook.yml
```

