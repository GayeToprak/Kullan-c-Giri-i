# Kullan-c-Giri-i

import java.util.Scanner;

public class sifre {
    public static void main(String [] args){
        String userName , password;
        String yeniSifre = "2";
        int secenek = 0;
        Scanner inp = new Scanner(System.in);

        System.out.print("kullanıcı adınız:");
        userName = inp.nextLine();

        System.out.print("şifreniz:");
        password = inp.nextLine();

        if(userName.equals("gaye")&& password.equals("gaye123")) {
            System.out.println("giriş yaptınız!");
        }else {
            System.out.println("şifreniz yanlış değiştirmek isterseniz 1' basınız:");
            secenek = inp.nextInt();

        }
        if (secenek == 1) {
           System.out.println("yeni şifreyi giriniz");
           yeniSifre = inp.next();

              if(yeniSifre.equals("gaye123")) {
                  System.out.println("şifre oluşturulamadı farklı bir şifre oluşturunuz.");
                  yeniSifre = inp.next();
                  System.out.println("şifreniz başarıyla değiştirildi.");

                }else{
                    System.out.println("şifreniz başarıyla değiştirildi.");
              }


        }
    }
}
