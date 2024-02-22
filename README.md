# verificaseumnumeroeprimo



package verificanumeroprimo;

 import java.util.Scanner;

public class VerificaNumeroPrimo {

    
    public static void main(String[] args) {
        
  Scanner Scanner =  new Scanner (System.in);    

// solicita ao usuario que insira um numero 
        System.out.println("Digite um número inteiro maior que 1:");
        int numero =Scanner.nextInt();
         
        // verifica se o número é primo
        boolean ehprimo = true;
        if(numero<=1){
            ehprimo=false;
        }else{
            for (int i= 2; i<= Math.sqrt(numero); i ++ ){
         
         if (numero% i==0){ 
        ehprimo= false;
        break;
         }              
            }
        }
        // exibe o resultado 
        
        if(ehprimo){
            System.out.println( numero + "é um número primo");
        }else{
            System.out.println(numero + " não é um número primo.");
        }
        // fecha o Scanner
        Scanner.close();
        
                
    }
    
}
