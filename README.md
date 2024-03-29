***PROGRAMIN İŞLEVİ***

Text Correction, Türkçe Otomatik Metin Düzenleme programıdır. NLP kütüphanesi kullanılarak,veri analizi yapılmaktadır.Veri tabanındaki veriler cümlelere ve kelimelere ayrılarak ,öğeler tespit edilir,kelimelerin birbirleriyle mantıksal bağlamları kurulur.

Program girdi olarak aldığı kelimelerden eksik ya da hatalı olanları doğru olanıyla değiştirir ve girilen cümleyi düzelterek kullanıcıya döndürür.

Program geliştirilmekte olduğu için bu aşamada sadece kelimeleri düzeltmektedir. Cümle bazında düzeltmeler için metot eklemeleri devam edecektir.

***PROGRAMDAKİ METOTLAR***

**main.py:** Programı yöneten ana metottur.

**createList.py:** Veri setini etiketleyen metottur.

**data_register.py:** Veri setini database kaydeden ara metottur.

**otoset.py:** Eksik ya da yanlış girilen kelimeler için veri tabanındaki yakın kelimeleri bulan metottur.

**database.py:** Database tablosu oluşturan ve etiketlenen veriyi tabloya kaydeden metottur.

**data.db:** Program tarafından oluşturulan database dosyasıdır.Bu dosyayı açmak için ,işletim sistemine uygun olan "sqlLite veri tabanı motoru" indirilmelidir.

**text.py:** Veri setini tutar.

**pos_tag:** Bu fonksiyon sayesinde, cümlemizdeki özel isimleri, sıfatları vb. bulabiliriz.

**stop_words:** Metinden bir öznitelik çıkarımı yaparken herhangi bir önem taşımayan kelimelerden kurtulunur.

**text_cleaning:** Metni noktalama işaretlerinden ve özel karakterlerden arındırmak. 

**tokenization:** Ham metni cümle ve kelimelere ayırır.

**wordnet:** İki kelimenin birbirine olan benzerlik oranını hesaplar.

***PROGRAMIN ÇALIŞTIRILMASI***

Programı VsCode ile çalıştırmak için:

1)cmd açılır.

2)python -m venv <myenv vs. gibi bir dosya adı verilir>

3)"myenv/Scripts/activate" komutu ile dosyaya girilir.

4)"pip install numpy" komutu ile numpy kütüphanesi kurulur.

5)"pip install nltk" komutu ile nltk kütüphanesi kurulur.

6)her bir .py uzantılı dosya "python <dosya adı>.py" gibi komutlarla çalıştırılır.

örneğin; "python wordnet.py"

7)"pip install fuzzywuzzy"
  "pip install python-Levenshtein" komutları ile fuzzywuzzy kütüphanesi indirilmelidir.Bu kütüphane iki kelimeyi karşılaştırarak benzerlik oranını hesaplar.

***PROGRAM ARAYÜZÜ***

**mesaj girin:** Kullanıcının kelime girdisi yapacağı alandır.Her girilen karakterden sonra yeni cümle önerileri yapılır.

**öneriler:** Girdi olarak eksik ya da yanlış yazılan kelimelere uygun sonuçların döndürüldüğü alandır.Uygun sonuçlardan en fazla 4 tanesi döndürülür.

**temizle butonu:** Arayüzü temizler.
