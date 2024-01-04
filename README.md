# KDV
KDV tutarını hesaplayan program.
package patikaAcademy;

import java.util.Scanner;

public class kdvHesaplama {

	public static void main(String[] args) {
     
		Scanner input = new Scanner(System.in);
		
		double fiyat ;
		
		
		
		System.out.println("Fiyatı giriniz ");
		fiyat= input.nextInt()	;
		
		boolean sonuc = fiyat <1000;
		double kdv = sonuc ? 0.18 : 0.08 ;
		
		double kdvTutari= fiyat * kdv ;
		double sonFiyat= kdvTutari+ fiyat;
		
		System.out.println("KDV tutari="+ kdvTutari);
		System.out.println("KDV'li fiyat="+ fiyat);
