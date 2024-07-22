1. Dopo aver importato il template di base della repository lancio i comandi npm install e composer install. Creo poi il file ".env", lo collego al DB creato in precedenza e creo infine la chiave col comando php artisan key:generate. Lancio poi i compandi npm run dev e php artisan serve.

2. Creo in (app -> http -> contollers) un controller col comando "php artisan make:controller ColorsController".

3. Creo in (app -> models) un model col comando "php artisan make:model Color".

4. Creo poi in (database -> migrations) una migrazione col comando "php artisan make:migration create_colors_table". Qui inserisco 4 colonne: red, blue, green e opacity. Assegno poi i rispettivi valori accettabili (per i primi 3, dei numeri da –32,767 a +32,767. Per l'ultimo, dei numeri decimali composti da un totale di 2 cifre, di cui una dopo la vorgola, ovvero da 0,0 a 9,9). 
Lancio poi la migrazione per generare la tabella nel DB col comando "php artisan migrate"