# Granada CF 
## El Granada CF se fundo el 6 de abril del año 1931
### Este año jugamos en segunda division

El **Granada CF** jugo el año pasado en *primera division y descendio.* Actualmente en la temporada **2024/25** juega en Segunda.

[Escudos historias](hisotria.png)

![1931](URL_de_la_imagen)

6 Jugadores del Granada  
1. Uzuni
2. El Arabi
3. Ighalo
- Batalla.
- Sergio Ruiz
- Brahimi

| Nombre | Apellido | DNI |
|--------|----------|-----|
|Oliver  |Montes Marcos| 77147010L |

>En 1931 un gran club de futbol
      
        Scanner teclado = new Scanner(System.in);
        int opcion = 0;
        
        while (opcion != 5) {
            System.out.println("1. Suma");
            System.out.println("2. Resta");
            System.out.println("3. Multiplicación");
            System.out.println("4. División");
            System.out.println("5. Salir");
            System.out.print("Seleccione una opción: ");
            
            opcion = teclado.nextInt();
           
            if (opcion >= 1 && opcion <= 4) {
                System.out.print("Introduce el primer número: ");
                int numero1 = teclado.nextInt();
                System.out.print("Introduce el segundo número: ");
                int numero2 = teclado.nextInt();

                switch (opcion) {
                    case 1: 
                        System.out.println("Resultado de la suma: " + (numero1 + numero2));
                        System.exit(0);
                        break;
                    case 2:
                        System.out.println("Resultado de la resta: " + (numero1 - numero2));
                        System.exit(0);
                        break;
                    case 3: 
                        System.out.println("Resultado de la multiplicación: " + (numero1 * numero2));
                        System.exit(0);
                        break;
                    case 4:
                        if (numero2 != 0) {
                            System.out.println("Resultado de la división: " + ((double)numero1 / numero2));
                        } else {
                            System.out.println("Error: No se puede dividir por cero.");
                           System.exit(0);
                        }
                        break;
                }
            } else if (opcion != 5) {
                System.out.println("Opción no válida. Intente de nuevo.");
            }
        }
        System.out.println("Programa finalizado.");
    }
}
