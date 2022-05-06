# venta-por-comision-java
Sistema comision por Venta en java
public class Venta {
/*Sistema comision por Venta en java*/
    public static void main(String[] args) {
 /* Esta son las Variables que declaramos*/
        int Sueldo, Venta, Comision;
      /*Ingresar el sueldo por Teclado*/
        System.out.println("Favor ingresar el sueldo");
        /* captura de la informacion enviada por el teclado*/
        Scanner tecla = new Scanner(System.in);
        /*almacenando la informacion en la variable sueldo ingresada por teclado */ 
        Sueldo = tecla.nextInt();
        /* captura de la informacion enviada por el teclado*/
        System.out.println("Favor ingresar la venta");
          /* captura de la informacion enviada por el teclado*/
        tecla = new Scanner(System.in);
         /*almacenando la informacion en la variable Venta ingresada por teclado */ 
        Venta = tecla.nextInt();
        /*almacenando la informacion en la variable sueldo ingresada por teclado */ 
        if (Venta<=100000) {
            System.out.println("el vendedor no tiene comision  teniendo en cuenta que no supero  la meta ");
             /*Condicional si la venta es mayor a 100000 mil */ 
        } else if (Venta > 100000.){
            /* la comision sera el  10% de las venta  */
            Comision = (int) (Venta*0.10);
            System.out.println(Comision+Sueldo);
        }
         /*Condicional si la venta es mayor o igual  a 1000000 un millon */
        else if (Venta>=1000000) {
             /* la comicion sera el  5% de las venta  */
            Comision = (int) (Venta*0.05);
        } 
        else {
            System.out.println("Finalizando el Systema");
        }
            
        }}
