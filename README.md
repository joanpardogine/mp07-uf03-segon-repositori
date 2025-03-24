# **Activitat: Segon repositori amb Visual Studio Code**

## **Objectiu**

Aprendre a:

✅ Comprovar que **Git** i **Visual Studio Code** estan instal·lats i configurats correctament.  
✅ Configurar **Visual Studio Code** perquè utilitzi **Git Bash** com a terminal per defecte.  
✅ Crear una estructura de carpetes ordenada a **`C:\projectes`**.  
✅ Crear un repositori nou a **GitHub** i clonar-lo.  
✅ Utilitzar **Markdown** correctament per documentar el projecte.  
✅ Entendre la importància dels **commits** i fer-los correctament.  
✅ Fer servir **Git Bash** dins del *terminal* de **VS Code** per totes les operacions de **Git**.  

---

## **Pas 1: Comprovació de la instal·lació i configuració**

### **Explicació**

Abans de començar, assegurem-nos que tenim tot el necessari per treballar. Això evitarà problemes més endavant.

### **Instruccions**
1. **Obrir Visual Studio Code**.
2. Anar a **View > Terminal** (o prémer `Ctrl + J`).
3. Si el terminal que s'obre **NO** és **Git Bash**, cal configurar-lo:
   - Fes clic a la petita fletxa a la part superior del terminal.
   - Selecciona **Select Default Profile**.
   - Tria **Git Bash**.
   - Tanca el terminal (`X`) i torna a obrir-lo (`Ctrl + J`).
4. **Verificar que Git està instal·lat** escrivint:
   ```bash
   git --version
   ```
   Ha de mostrar una versió com `git version 2.x.x`.  
   Si no, cal instal·lar Git.
5. **Comprovar la configuració d’usuari** amb:
   ```bash
   git config --list
   ```
   Ha de mostrar el teu nom i correu electrònic (si no, cal configurar-los).

<details><summary> Pitja per veure com configurar-los</summary>

### Configurar Git per primera vegada

Abans de començar a treballar amb **Git**, hem de configurar-lo perquè ens identifiqui correctament.

Això permetrà que cada canvi que fem quedi registrat amb el nostre nom i correu electrònic.

Instruccions

1. **Obrir Visual Studio Code**.
2. Anar a **View > Terminal** (o prémer `Ctrl + J`).
3. Escriu les següents comandes, substituint "**`El teu nom`**" i "**`el_teu_email@example.com`**" pel teu **usuari de `github`** i el teu **correu**:

```bash
git config --global user.name "El teu nom"
git config --global user.email "el_teu_email@example.com"
```

Comprova que la configuració s’ha guardat correctament amb:

```bash
git config --list
```

Ha de mostrar el teu nom i correu.

</details>

---

## **Pas 2: Crear una estructura de carpetes ordenada**
### **Explicació**
Treballar amb una estructura clara ens ajudarà a no perdre els nostres projectes.

### **Instruccions**
1. **Obrir el terminal de Git Bash** dins de VS Code.
2. Escriure la següent comanda per anar a `C:`:
   ```bash
   cd /c
   ```
3. Crear una carpeta anomenada `projectes` (si no existeix):
   ```bash
   mkdir projectes
   ```
4. Entrar dins la carpeta:
   ```bash
   cd projectes
   ```
5. Per comprovar que la carpeta s’ha creat correctament, fer:
   ```bash
   ls
   ```
   Si `projectes` apareix a la llista, tot està correcte.

---

> 
> ### Com que farem més projectes al llarg del curs, guardarem tots els treballs en una mateixa carpeta (`C:\projectes`). Això ens facilitarà trobar-los ràpidament i seguir un ordre com fan els professionals.
>

---

## **Pas 3: Crear un repositori a GitHub i clonar-lo**
### **Explicació**
Un **repositori** és com una carpeta especial on guardem el nostre codi i l’historial de canvis.

### **Instruccions**
1. Anar a **GitHub** i iniciar sessió.
2. Crear un **New Repository** amb nom **`segon-repositori`**.
3. **NO marcar** "Add a README file".
4. Clicar **Create repository**.
5. Copiar l’enllaç que proporciona GitHub (**`https://github.com/el-teu-usuari/segon-repositori.git`**).
6. **Obrir el terminal de Git Bash** dins de VS Code.
7. Escriure la següent comanda per anar a `C:`:
   ```bash
   cd /c
   ```
8. clonar el repositori:
   ```bash
   git clone https://github.com/el-teu-usuari/segon-repositori.git
   ```
9. Entrar a la carpeta creada:
   ```bash
   cd segon-repositori
   ```
---

## **Pas 4: Crear i editar el fitxer README.md**

### **Explicació**

El fitxer **`README.md`** serveix per descriure el projecte i explicar de què tracta.

### **Instruccions**

1. A **VS Code**, crear un fitxer nou anomenat **`README.md`**.
2. Escriure el següent contingut:
   ```markdown
   # El meu primer projecte amb GitHub
   Aquest és un projecte de pràctica per aprendre Git, GitHub i Markdown.

   ## Markdown bàsic
   **Negreta**, *cursiva*, i [un enllaç a Google](https://www.google.com).
   ```
3. Desa el fitxer (`Ctrl + S`).

---

## **Pas 5: Fer el primer commit**
### **Explicació**
Un **commit** guarda els canvis del nostre projecte. Fer commits sovint ens ajuda a tenir un historial clar i recuperar versions anteriors si cal.

👉 **Quan s'ha de fer un commit?**  
- Cada cop que es completa una part del projecte.  
- Si s’ha fet un canvi important.  
- Abans de fer modificacions grans.  

**Mala pràctica:** Fer només un commit quan s'acaba el projecte.  
**Bona pràctica:** Fer **commits petits i freqüents**.

### **Instruccions**
1. **Comprovar l'estat del repositori**:
   ```bash
   git status
   ```
2. **Afegir els canvis per al commit**:
   ```bash
   git add README.md
   ```
3. **Fer el commit amb un missatge explicatiu**:
   ```bash
   git commit -m "Afegit el fitxer README.md amb exemples de Markdown"
   ```
4. **Pujar el commit a GitHub**:
   ```bash
   git push origin main
   ```

---

## **Conclusió**
✅ Han confirmat que tenen Git i VS Code configurats correctament.  
✅ Han après a **usar Git Bash dins de VS Code**.  
✅ Han creat una estructura de carpetes clara (**`C:\projectes`**).  
✅ Han creat un repositori i l’han clonat.  
✅ Han après Markdown i les seves opcions de formatació.  
✅ Han entès la importància de fer **commits freqüents i explicatius**.  

---
