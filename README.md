# Práctica Git & GitHub - RESPUESTAS

### 📌 Paso 11: ¿Qué comando utilizaste en el paso 11? ¿Por qué?
```bash
git reset --hard HEAD~1
```
**Explicación:**
Este comando deshace el último commit, eliminando los cambios del working copy y el staging area. Se usa `--hard` para borrar completamente los cambios.

---

### 📌 Paso 12: ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
```bash
git reflog
git reset --hard <ID_DEL_COMMIT>
```
**Explicación:**
- `git reflog`: Muestra el historial de commits recientes, incluyendo el que deshicimos.
- `git reset --hard <ID_DEL_COMMIT>`: Permite volver al commit eliminado, restaurando los cambios.

---

### 📌 Paso 13: ¿El merge causó algún conflicto? ¿Por qué?
**Comando utilizado:**
```bash
git merge main
```
**Respuesta:**
En principio no hubo conflictos porque la rama main no tenía nuevos cambios en comparación con la rama actual. Sin embargo, después de agregar nuevos cambios en la rama main, se produjeron conflictos al intentar fusionarla nuevamente. Esto se debe a que los nuevos cambios introducidos en main no coincidían con las modificaciones en la rama actual.

---

### 📌 Paso 19: ¿El merge causó algún conflicto? ¿Por qué?
**Comando utilizado:**
```bash
git checkout styled
git merge htmlify
```
**Respuesta:**
Poorque ambas ramas, styled y htmlify, tenían cambios que afectaban las mismas partes del .md. Cuando git intentó fusionar estas diferencias, no pudo hacerlo automáticamente y necesitó intervención manual para resolver los conflictos.

---

### 📌 Paso 21: ¿El merge causó algún conflicto? ¿Por qué?
**Comando utilizado:**
```bash
git checkout main
git merge styled
```
**Respuesta:**
No hubo conflicto, porque no hubo un cambio significativo en el .md y git puede manejar los merges automáticamte siempre que no haya modificaciones solpadas en las mismas partes del archivo.

---

### 📌 Paso 25: ¿Qué comando o comandos utilizaste en el paso 25?
```bash
git log --graph --oneline --all
```

### 📌 Paso 26: ¿El merge podría ser fast forward? ¿Por qué?
**Comando utilizado:**
```bash
git checkout main
git merge --no-ff title -m "Fusionar title en main"
```
**Respuesta:**
Si, Porque `main` no ha cambiado desde que se creó `title`**, en cuyo caso `main` simplemente avanzaría sin crear un nuevo commit de merge.

---

### 📌 Paso 27: ¿Qué comando o comandos utilizaste en el paso 27?
```bash
git reset --merge HEAD~1
```

### 📌 Paso 28: ¿Qué comando o comandos utilizaste en el paso 28?
```bash
git checkout -- .
```

### 📌 Paso 29: ¿Qué comando o comandos utilizaste en el paso 29?
```bash
git branch -d title
```
**Nota:**
Aunque hubo una rama que no se podía eliminar porque la rama no ha sido fusionada, lo cual tenía que forzar con el siguiente comando:
```bash
git branch -D title
```

### 📌 Paso 30: ¿Qué comando o comandos utilizaste en el paso 30?
```bash
git merge --no-ff title -m "Rehacer merge de title"
```

### 📌 Paso 32: ¿Qué comando o comandos usaste en el paso 32?
```bash
git checkout <ID_DEL_COMMIT_INICIAL>
```

### 📌 Paso 33: ¿Qué comando o comandos usaste en el punto 33?

```bash
git checkout title
```


