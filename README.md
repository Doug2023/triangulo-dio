# triangulo-dio

import java.io.IOException;
import java.util.Scanner;

public class Triangulo {
    public static void main(String[] args) throws IOException {
        Scanner leitor = new Scanner(System.in);
        double A = leitor.nextDouble();
        double B = leitor.nextDouble();
        double C = leitor.nextDouble();
        double maior = A;
        double soma = C + B;
        boolean triangulo = soma > maior;
        double perimetro = A + B + C;
        double areaTrapezio = ((A + B) * C) / 2;

        if (triangulo){
            System.out.printf("Perimetro = %.1f%n", perimetro);
        } else {
            System.out.printf("Area = %.1f%n", areaTrapezio);
        }
    }
}
