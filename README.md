# Piattaforma Eventi

## Clonare il Progetto

Per clonare il progetto completo con tutti i submodule:

```bash
git clone --recursive https://github.com/TUO_USERNAME/piattaforma_eventi.git
```

## Struttura del Progetto

- `p_e_front/` - Frontend Angular
- `p_e_back/` - Backend NestJS

## Aggiornare i Submodule

Per aggiornare tutti i submodule all'ultima versione:

```bash
git submodule update --remote
```

## Sviluppo

### Frontend

```bash
cd p_e_front
npm install
ng serve
```

### Backend

```bash
cd p_e_back
npm install
npm run start:dev
```
