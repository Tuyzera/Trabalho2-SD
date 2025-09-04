# Trabalho2-SD
Arthur Utpadel e Kevin Schops Cavalheiro

# Algoritmo de Berkeley – Sincronização de Relógios --- ## 📂 Estrutura do Projeto
berkeley_sync/
 ├── common.py  
 ├── server.py   
 ├── client.py
--- ## 🚀 Como Executar ### 1. Inicie o Servidor Abra um terminal e rode:
bash
python server.py --clients 3
Isso inicia o servidor, esperando **3 clientes** se conectarem. Você pode usar --interval N para repetir a sincronização a cada **N segundos**:
bash
python server.py --clients 3 --interval 10
--- ### 2. Conecte os Clientes Em terminais separados, execute cada cliente com um nome e offset inicial:
bash
python client.py --name A --offset 5
python client.py --name B --offset -3
python client.py --name C --offset 12
- --name define o nome do cliente. - --offset define o deslocamento inicial do relógio (em segundos). ---
