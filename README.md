# Descoperirea puterii containerelor

## Intenție

Această experiență de laborator este gândită pentru a introduce utilizatorii în funcționarea OS-urilor Debian/Ubuntu și pentru a-i iniția în lumea Docker și a comenzilor sale fundamentale.

## Prezentare

Plecat de la imaginea oficială a sistemului de operare Ubuntu, vom construi un container ce va găzdui un server web Apache. Vom crea o pagină web simplă ce va afișa mesajul "Hello, World!" și vom testa accesarea acesteia într-un browser.

## Pași de urmat

1. **Inițiere și verificare:**

   Pornim terminalul în directorul 'containers03' și executăm comanda de mai jos pentru a demara un container Ubuntu și a accesa terminalul său interactiv:

   ```bash
   docker run -ti -p 8000:80 --name containers03 ubuntu bash
   ```bash
*   **Obiectiv:** Această comandă lansează un container Docker bazat pe imaginea Ubuntu și ne conectează la terminalul său.
*   **Rezultat:** Suntem acum în terminalul containerului, pregătiți pentru a executa comenzile necesare.

În terminalul containerului, rulăm următoarele comenzi:

```bash
apt update
