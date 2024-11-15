### README - Sistema Sense-and-Avoid per Droni con Resilienza agli Attacchi Numb

#### **Titolo del Progetto**
Modellazione e Analisi del Comportamento Sense-and-Avoid per Droni in Presenza di Attacchi Numb e Interruzioni della Rete 4G

---

#### **Descrizione**
Il progetto analizza l’implementazione e la verifica formale di un sistema di sense-and-avoid (SAA) per droni, focalizzandosi su scenari che includono interruzioni di rete e attacchi informatici come il Numb Attack. Il comportamento del drone è modellato attraverso metodi formali che includono transizioni di stato, variabili ambientali e specifiche logiche temporali, al fine di garantire operazioni sicure e robuste.

---

#### **Caratteristiche Principali**
- **Sistema Sense-and-Avoid**:
  - Utilizzo di sensori avanzati (radar, lidar, telecamere) per rilevamento e evitamento ostacoli in tempo reale.
  - Decisioni autonome in ambienti complessi.

- **Attacco Numb**:
  - Analisi delle minacce che compromettono i dati dei sensori, riducendo la capacità del drone di rilevare ostacoli.
  - Strategie di mitigazione per garantire sicurezza operativa.

- **Comportamento in Assenza di Rete**:
  - Studio delle risposte del drone (atterraggio di emergenza, ritorno alla base) in caso di perdita della connettività 4G.

- **Verifica Formale**:
  - Implementazione di logiche temporali CTL (Computation Tree Logic) e LTL (Linear Temporal Logic) per la verifica delle proprietà del sistema.
  - Validazione di requisiti critici come l’evitamento degli schianti e l’uso efficiente delle risorse.

---

#### **Stati del Sistema**
Il drone opera attraverso stati predefiniti:
1. **Normale**: Operazione standard.
2. **No Rete**: Perdita della connessione 4G.
3. **Atterraggio**: Discesa d’emergenza.
4. **Ritorno alla Base**: Navigazione verso il punto di partenza.
5. **Schianto**: Fallimento operativo con impatto.
6. **Manutenzione**: Controllo o riparazione del sistema.
7. **Tentativo di Riconnessione**: Tentativo di ristabilire la rete.
8. **Errore di Riconnessione**: Fallimento dopo più tentativi di riconnessione.
9. **Manutenzione Programmata**: Manutenzione pianificata.
10. **Emergenza**: Stato attivato in condizioni avverse (es. meteo sfavorevole).

---

#### **Punti Salienti della Modellazione**
- **Transizioni di Stato**: Definite tramite logiche condizionali che considerano rete, meteo e livello di batteria.
- **Gestione della Batteria**: Monitoraggio del consumo con azioni di sicurezza in caso di livelli critici.
- **Variabili Ambientali**: Condizioni meteorologiche e di rete che influenzano le decisioni.

---

#### **Obiettivi della Verifica**
1. **Sicurezza**: Assicurarsi che il drone eviti sempre collisioni.
2. **Autonomia**: Validare la capacità del drone di gestire problemi in modo indipendente.
3. **Efficienza**: Ottimizzare le decisioni per l’uso di batteria e risorse.
4. **Resilienza**: Dimostrare robustezza contro attacchi come il Numb Attack.

---

#### **Tecnologie**
- **Strumenti di Modellazione**: NuSMV per la specifica e la verifica formale.
- **Logiche di Verifica**: CTL e LTL per esprimere proprietà di sicurezza e vivacità.

---

#### **Utilizzo**
1. Simulare vari scenari (es. perdita di rete, attacchi Numb) per testare il comportamento del drone.
2. Utilizzare strumenti di verifica formale per garantire la conformità delle proprietà di sistema.
3. Analizzare i risultati per migliorare il modello e aumentare la resilienza del sistema.

---

