## **READ ME!!**
---

### **Panoramica dei Branch**

- **`main`**:  
  Il **branch principale** dove mettiamo solo versioni finali e stabili del progetto.  
  **Non fare il push su `main`**; tutte le modifiche passano su `develop`.

- **`develop`**:  
  Questo è il **branch di integrazione** dove mettiamo insieme il lavoro di tutti prima di consegnare. È il branch più aggiornato e completo.  
  Ognuno di noi deve lavorare sui propri branch personali, e poi fare la merge in `develop`.

- **Branch personali** (`Luke-Branch`, `Jonny-Branch`, `Samu-Branch`, `SDL-Branch`):  
  Ognuno di noi ha un **branch personale**.  
  **Non fare il push direttamente su `develop`**. Prima crea una Pull Request (PR) dal tuo branch al branch `develop`.

---

### **Cosa dovremmo fare**

1. **Prima di tutto, assicurarci di essere su `develop`**:
   ```bash
   git checkout develop
   git pull origin develop
   ```

2. **Addare - committare - pushare le modifiche su `tua-branch`**:
   ```bash
   git add .
   git commit -m "Descrivi brevemente cosa hai fatto - cose sensate!!"
   git push origin tuo-branch
   ```

3. **Creare una Pull Request (PR) su `develop` dal `tua-branch`** (così possiamo fare una revisione)

4. **Mergiare le nostre branch in `develop`** (dopo che abbiamo approvato ihih)
   Non mergiate direttamente in `main`!!!

5. **Tenete sempre aggiornato `develop`**:
   ```bash
   git checkout develop
   git pull origin develop
   ```

6. **Alla fine di tutto aggiungiamo il file finale (group2508_exerciseX.ipynb) in `main`** :)

---

### **NON FARE:**  
- **Non fare il push direttamente su `main` o `develop`.**
- Tutte le modifiche devono passare per una **Pull Request** e essere revisionate prima della merge.

---

### **Comandi Git Utili**  
- **Controlla il branch su cui ti trovi**:
  ```bash
  git branch
  ```

- **Cambia branch**:
  ```bash
  git checkout nome-del-branch
  ```

- **Crea un nuovo branch**:
  ```bash
  git checkout -b nuovo-nome-branch
  ```

- **Prendi gli aggiornamenti dal repository remoto**:
  ```bash
  git pull origin nome-del-branch
  ```

- **Fai il push delle modifiche su GitHub**:
  ```bash
  git push origin nome-del-branch
  ```

- **Vedi lo stato dei file**:
  ```bash
  git status
  ```

- **Committa le modifiche**:
  ```bash
  git add .
  git commit -m "Messaggio del commit"
  ```

- **Mergia un branch**:
  ```bash
  git merge nome-del-branch
  ```

- **Elimina un branch**:
  ```bash
  git branch -d nome-del-branch  # Elimina localmente
  git push origin --delete nome-del-branch  # Elimina remotamente
  ```
