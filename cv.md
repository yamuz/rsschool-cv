# **ABDRAYEV ALMAZ**
FRONTEND/ANDROID Developer

Almaty,Kazakhstan, Cell(+77082587588),(yamuuzz@gmail.com)

![almaz_small](https://user-images.githubusercontent.com/5288027/133981647-6daccb0c-25fa-45ab-ae21-567bd20ffd26.jpg)


# **EXPERIENCE**
* Clinic Mobile app for Android (making an appointment to the doctor)
* Cargo Mobile app for Android (for ordering a taxi/cargo vehicle)

# **EDUCATION**
 * ITMO UNIVERSITY (https://itmo.ru/), BSc Optoelectonics, 2007
 * Applications for Handheld Systems, Coursera MOOC, 2015
 * Java Basics, Online, [javarush.ru](www.javarush.ru), 2021- still going (22 lvl)
 * RS SChool FrontEnd, Online,(https://rs.school/)
 
# **SKILLS**
 * Android Studio
 * Java (SE)
 * MS SQL, SQLite
 * html, css
 * javascript
 * git
 
# **LANGUAGES**
 * English: intermediate ( estimated unofficially IELTS 6 : reading 6, speaking 5, writing 6, listening 6.5), constantly improving my language skills

# **CODE SAMPLES

**JAVASCRIPT**:

function absentVowel(x){
                        const vowels = new Map([["a",0],["e",0], ["i",0], ["o",0], ["u",0]])
                    
                        for (let word of x.split(" ")){
                            for (let vowel of vowels.keys()){
                                if (word.toLowerCase().indexOf(vowel) != -1 )
                                   vowels.set(vowel, vowels.get(vowel) +1)         
                            }
                        }
                        
                        let indices = ["a","e","i","o","u"]
                        for (let vowel of vowels.keys()){
                            console.log(vowel + " : " + vowels.get(vowel))
                            if (vowels.get(vowel)===0)
                                return indices.indexOf(vowel);    
                        }
                    
                        return NaN;
}

**JAVA**:

import java.io.*;
import java.util.zip.*;  
public class Program {
  
    public static void main(String[] args) {
         
        String filename = "C:\\SomeDir\\notes.txt";
        try(ZipOutputStream zout = new ZipOutputStream(new FileOutputStream("C:\\SomeDir\\output.zip"));
                FileInputStream fis= new FileInputStream(filename);)
        {
            ZipEntry entry1=new ZipEntry("notes.txt");
            zout.putNextEntry(entry1);
            
            byte[] buffer = new byte[fis.available()];
            fis.read(buffer);
            zout.write(buffer);
            zout.closeEntry();
        }
        catch(Exception ex){     
            System.out.println(ex.getMessage());
        } 
    } 
}
