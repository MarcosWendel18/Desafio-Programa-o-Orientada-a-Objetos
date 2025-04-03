# Desafio-Programa-o-Orientada-a-Objetos

import java.util.Scanner;

public class Aumento_salarial {
    public static void main(String[] args) {
        Scanner ent = new Scanner(System.in);
        double Salario = 0.0;
        double Aumento = 0;
        double Salariof;
        double Salariofi;
        int i = 0;
        System.out.println("Informe o valor do seu salário: ");
        Salario = ent.nextDouble();
        if(Salario <= 280) {
            Aumento = Salario * 0.20;
            i = 20;
        }if(Salario > 280 && Salario < 700){
            Aumento = Salario * 0.15;
            i = 15;
        }if(Salario >= 700 && Salario < 1500){
            Aumento = Salario * 0.10;
            i = 10;
        }if(Salario > 1500) {
            Aumento = Salario * 0.05;
            i = 5;
        }Salariof = Salario + Aumento;
        Salariofi = Salariof -(Salariof * 0.038);
        System.out.println("\n Valor do salário antigo: R$"+ Salario +"\n Percentual aumentado: "+ i +"%"+"\n Valor do aumento; "+ Aumento +"\n Valor do novo salário: R$"+ Salariof +"\n Valor do aumento menos valor da inflação: R$"+ Salariofi);
    }
}
