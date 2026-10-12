import java.util.Scanner;
public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Escribe una palabra o texto corto: ");

        String texto = sc.nextLine();
        //String texto: Guarda el texto escrito//

        String resultado = "";

        for (int i = texto.length() - 1; i >= 0; i--) {
            //texto.length(): Obtiene la cantidad de caracteres//
            //for: Recorre el texto desde el último carácter hasta el primero//

            resultado += texto.charAt(i);
            //charAt(i):Obtiene el carácter que corresponde a la posición//
            //resultado += : Va formando el texto invertido//
        }
        System.out.println("Texto transformado: " + resultado);

        sc.close();
    }
}
//El programa recibe un texto y lo muestra en orden inverso//