# burc
patika.dev burc bulan program

import java.util.Scanner;
public class main {
    public static void main(String[] args){
        int month, day;
        String burc="";
        boolean isError = false;
        System.out.println("Kaçıncı ayda doğdunuz?");
        Scanner inp = new Scanner(System.in);
        month = inp.nextInt();
        
        System.out.println("Ayın kaçında doğdunuz?");
        day = inp.nextInt();

        switch (month){
            case 1:
                if (day >=1 && day <= 31){
                    if (day < 22) {
                        burc = "Oğlak";
                    }else{
                        burc = "Kova";
                    }
                }else{
                    isError = true;
                }
                break;
            case 2:
                if (day >=1 && day <= 29){
                    if (day < 19) {
                        burc = "Kova"; 
                    }else{
                        burc = "Balık";
                    }
                }else{
                    isError = true;
                }
                break;
            case 3:
                if (day >=1 && day <= 31){
                    if (day < 20) {
                        burc = "Balık";
                        burc = "Koç";
                    }
                }else{
                    isError = true;
                }
                break;
            case 4:
                if (day >=1 && day <= 30){
                    if (day < 21) {
                        burc = "Koç";
                    }else{
                        burc = "Boğa";
                    }
                }else{
                    isError = true;;
                }
                break;
            case 5:
                if (day >=1 && day <= 31){
                    if (day < 22) {
                        burc = "Boğa";
                    }else{
                        burc = "İkizler";
                    }
                }else{
                    isError = true;
                }
                break;
            case 6:
                if (day >=1 && day <= 30){
                    if (day < 23) {
                        burc = "İkizler";
                    }else{
                        burc = "Yengeç";
                    }
                }else{
                    isError = true;
                }
                break;
            case 7:
                if (day >=1 && day <= 31){
                    if (day < 23) {
                        burc = "Yengeç";
                    }else{
                        burc = "Aslan";
                    }
                }else{
                    isError = true;
                }
                break;
            case 8:
                if (day >=1 && day <= 31){
                    if (day < 23) {
                        burc = "Aslan";
                    }else{
                        burc = "Başak";
                    }
                }else{
                    isError = true;
                }
                break;
            case 9:
                if (day >=1 && day <= 30){
                    if (day < 23) {
                        burc = "Başak"; 
                    }else{
                        burc = "Terazi";
                    }
                }else{
                    isError = true;
                }
                break;
            case 10:
                if (day >=1 && day <= 31){
                    if (day < 23) {
                        burc = "Terazi";
                    }else{
                        burc = "Akrep";
                    }
                }else{
                    isError = true;
                }
                break;
            case 11:
                if (day >=1 && day <= 30){
                    if (day < 22) {
                        burc = "Akrep";
                    }else{
                        burc = "Yay";
                    }
                }else{
                    isError = true;
                }
                break;
            case 12:
                if (day >=1 && day <= 31){
                    if (day < 23) {
                        burc = "Yay";
                    }else{
                        burc = "Oğlak";
                    }
                }else{
                    isError = true;
                }
                break;
                default:
                isError = true;     
        }
        if(isError){
            System.out.println("Hatalı giriş yaptınız.");
        }else {
            System.out.println("Burcunuz=" + burc);
        }
        
    }  
}
