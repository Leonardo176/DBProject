# Requisiti

Note:

- indirizzo come stringa o composto?
- posizione enum (ricercatore, professore associato, professore ordinario).
- autori attributo lista oppure attributo a parte?
- scadenza per i prestiti?
- Mettere ripiano e scaffale in entità diverse

Lista entità:

- utente (KEY(codice), nome, cognome, indirizzo, facoltà)
- docente (KEY(utente), posizione)
- studente (KEY(utente), matricola)
- libro (KEY(ISBN), titolo, autori)
- copia (KEY(numero, libro), ripiano, scaffale)
- prestito (KEY(idPrestito), utente, copia, data/ora acquisizione, data/ora consegna)
- consultazione (KEY(idConsultazione), utente, copia, data/ora inizio, data/ora fine)
