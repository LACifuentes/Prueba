# Prueba

import java.util.Scanner;

public class Main {

    public static String decipher(String ciphertext, String knownWord) {
                String txt = ciphertext;
				String wrd = knownWord;
				char[] abc = new char[26];
				for ( int i=0 ; i < 26 ; i++) {
					abc[i] = (char) ('a' + i );
					//System.out.println(abc[i]);
				}
				for ( int i=0 ; i < txt.length() ; i++) {
					for (char c : abc) {
						if (c == txt.charAt(i)) {
							String nt = txt.replace("");
						}
					}
					//System.out.println(abc[i]);
				}
				
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String ciphertext = scanner.nextLine();
        String knownWord = scanner.nextLine();

        String result = decipher(ciphertext, knownWord);
        System.out.println(result);
    }
}
