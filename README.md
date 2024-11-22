# Piattaforma Eventi

Applicazione web per la gestione di eventi fotografici con sistema di votazione.

## Struttura del Progetto

- `p_e_front/` - Frontend Angular
- `p_e_back/` - Backend NestJS

## Requisiti

- Node.js
- Angular CLI
- MySQL

## Installazione

1. **Clona il repository con i submodule**

```bash
git clone --recursive https://github.com/franky-04/piattaforma_eventi.git
cd piattaforma_eventi
```

2. **Setup Backend**

```bash
cd p_e_back
npm install
# Configura il file .env con le tue variabili d'ambiente
npm run start:dev
```

3. **Setup Frontend**

```bash
cd p_e_front
npm install
ng serve
```

## Sviluppo

Quando lavori sui submodule, ricorda di:

1. Fare commit e push nelle rispettive cartelle dei submodule
2. Aggiornare i riferimenti nel repository principale:

```bash
git submodule update --remote
git add .
git commit -m "Update submodules"
git push
```

# Workflow Git per Progetti con Submodule

## 1. Modifiche al Frontend

```bash
# Naviga nella cartella frontend
cd p_e_front

# Fai le tue modifiche al codice
echo "// TODO: Implement login" >> src/app/login/login.component.ts

# Stage, commit e push delle modifiche
git add .
git commit -m "Added login component TODOs"
git push
```

## 2. Modifiche al Backend

```bash
# Naviga nella cartella backend
cd ../p_e_back

# Fai le tue modifiche al codice
echo "// TODO: Add auth middleware" >> src/middleware/auth.middleware.ts

# Stage, commit e push delle modifiche
git add .
git commit -m "Added auth middleware TODOs"
git push
```

## 3. Aggiorna il Repository Principale

```bash
# Torna alla cartella principale
cd ..

# Stage, commit e push dei riferimenti aggiornati dei submodule
git add .
git commit -m "Update: Added login and auth todos"
git push
```

## Verificare lo Stato

```bash
# Controlla lo stato dei submodule
git submodule status
```

## Note Importanti

### Da Ricordare

- Ogni submodule (frontend/backend) è un repository Git indipendente
- Devi fare commit/push sia nei submodule che nel repository principale
- Anche se lavori solo su un submodule, devi aggiornare il repository principale

### Comandi Utili

```bash
# Verifica lo stato dei submodule
git submodule status

# Se altri hanno fatto modifiche, aggiorna i submodule
git submodule update --remote

# Se hai appena clonato il progetto senza --recursive
git submodule update --init --recursive
```
