<!-- Aqui ponemos el titulo y con cada hastag que añadimos mas chico es el titulo -->
# Granada CF 
## El Granada CF se fundo el 6 de abril del año 1931
### Este año jugamos en segunda division

<!-- con dos astericos para abrir y cerrar ponemos la palabra en negrita y con una en cursiva-->
El **Granada CF** jugo el año pasado en *primera division y descendio.* Actualmente en la temporada **2024/25** juega en Segunda.

<!-- Para añadir una imagen en este caso pondremos un titulo cualquiera en los corchetes y despues añades el enlace de la foto de donde hayas descargado la imagen en github y lo pegas en los parantesis-->
[Escudos historias](hisotria.png)

<!-- Para añadir un enlace ponemos una exclamacion entre corchetes un titulo a la foto y el enlace de la imagen en los parantesis-->
![1931](hisotria.png)

<!-- Para añadir una lista ordenada pondremos los numeros con un punto y ya estaria ordenado-->
6 Jugadores del Granada  
1. Uzuni
2. El Arabi
3. Ighalo
<!-- Para poner puntos en vez de una lista ordenada con numeros solo tendremos que poner una raya y un espacio y ya saldria el puntito-->
- Batalla.
- Sergio Ruiz
- Brahimi

<!-- Para hacer una tabla pondremos los palos hacia abajo y para dividir pondriamos otro palo. Para ponerlo en hueco pondriamos el palo y las rayas y otro palo y ya estaria haciendo la tabla-->
| Nombre | Apellido | DNI |
|--------|----------|-----|
|Oliver  |Montes Marcos| 77147010L |

<!-- Para añadir una cita ponemos > y añadimos el texto que queramos -->
>En 1931 un gran club de futbol

<!-- Y para meter un codigo solo pondriamos una tabulacion y ya --> 
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
