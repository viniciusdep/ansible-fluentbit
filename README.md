# Fluent-bit automation using Ansible

Automação para instalação do Fluent-bit como serviço dentro dos hosts destino. Realiza automaticamente a checagem do sistema operacional e aplica o template correto. Seu OUTPUT padrão é o Opensearch, para mudanças, alterar a seção OUTPUT em templates/. 

## Installation

ansible-playbook -i hosts playbook.yml

```bash
Necessário criar arquivo de hosts
```

## Roles

```python
# Instalação do coletor
-  fluent-bit

# Parar o coletor
- stop-fluent-bit

```