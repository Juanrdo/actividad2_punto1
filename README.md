# actividad2_punto1

package empleado;
import java.util.Scanner;
public class Empleado {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        double  horastraba,valorhora,salnet,salbrut,retefu,codigo;
        Scanner ingresotecl = new Scanner (System.in);
        
        System.out.println("Ingrese el codigo:  ");
        codigo = ingresotecl.nextDouble();
        
        System.out.println("Ingrese los nombres:  ");
        String nombres = ingresotecl.next();
        
        System.out.println("Ingrese el numero de horas trabajadas al mes:  ");
        horastraba = ingresotecl.nextDouble();
        
        System.out.println("Ingrese el valor de la hora trabajada:  ");
        valorhora = ingresotecl.nextDouble();
        
        System.out.println("Ingrese el porcentaje de retencion:  ");
        retefu = ingresotecl.nextDouble();
        
        salbrut= horastraba*valorhora;
        salnet= salbrut - (salbrut *(retefu/100));
        
        System.out.println("el codigo es :  "+ codigo);
        System.out.println("los nombres son :  "+ nombres);
        System.out.println("el salario bruto es: "+ salbrut);
        System.out.println("el salario neto es :  "+ salnet);

    }
    

}
