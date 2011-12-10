---
layout: post
title: ActionScript Nedir? 2
---


ActionScript ile çalışma şekilleri

ActionScript'le çalışmanın birkaç yolu vardır.
- Komut Dosyası Yardımcısı modu ActionScript'i, kodu kendiniz yazmadan FLA dosyanıza
eklemenizi sağlar. Siz eylemleri seçersiniz ve yazılım her eylem için gerekli olan parametreleri
girmeniz amacıyla bir kullanıcı arabirimi sunar.
Belirli görevleri yerine getirmek için hangi işlevlerin kullanılacağı hakkında biraz bilginiz
olmalıdır ancak sözdizimi öğrenmenize gerek yoktur. Birçok programcı olmayan kişi ve
tasarımcı bu modu kullanmaktadır.

Örnek:

	function liste(urun:String) //fonksiyon içine parametre tanımladık.
	{
		trace("Alınacaklar listesi");
		trace("1-Deterjan");
		trace("2-Peyneri");
		trace("3-Süt");
		trace(urun)
	}
	liste("4-Çay");

kodun output ekranındaki çıktısı:
Alınacaklar listesi
1-Deterjan
2-Peyneri
3-Süt
4-Çay

- Davranışlar kodu kendiniz yazmadan dosyanıza eklemenizi sağlar. Davranışlar ortak görevler
için önceden yazılmış komut dosyalarıdır. Bir davranış ekleyebilir ve sonra onu Davranışlar
panelinde kolayca konfigüre edebilirsiniz. Davranışlar sadece ActionScript 2.0 ve önceki
sürümlerde bulunur.

- Kendi ActionScript'inizi yazmak size belgeniz üzerinde fazlasıyla esneklik ve kontrol sağlar
ancak ActionScript dili ve kurallarına aşina olmanız gerekir.

- Bileşenler, karmaşık işlevleri uygulamanıza yardımcı olan önceden oluşturulmuş film
klipleridir. Bir bileşen, onay kutusu gibi basit bir kullanıcı arabirimi kontrolü veya kaydırma
bölmesi gibi karmaşık bir kontrol olabilir. Bir bileşenin işlevini ve görünümünü özelleştirebilir ve
başka geliştiriciler tarafından oluşturulmuş bileşenleri indirebilirsiniz. Çoğu bileşen, bir bileşeni
tetiklemek veya kontrol etmek için bir miktar ActionScript kodu yazmanızı gerektirir.



Komut Dosyası Yardımcısı modu hakkında

ActionScript'e yeniyseniz veya ActionScript dilini ve sözdizimini öğrenmek zorunda kalmadan
basit etkileşim eklemek istiyorsanız, Eylemler panelindeki Komut Dosyası Yardımcısı'nı FLA
dosyalarınıza ActionScript eklemenize yardım etmesi için kullanabilirsiniz.

Komut Dosyası Yardımcısı, Eylemler araç kutusundan öğeler seçerek komut dosyaları
oluşturmanızı sağlar. Bir öğeyi bir defa tıklattığınızda, açıklaması panelin sağ üst tarafında
görünür. Bir öğeyi çift tıklattığınızda, öğe Eylemler paneli Komut Dosyası bölmesine eklenir.

Komut Dosyası Yardımcısı modunda, Komut Dosyası bölmesinde deyim ekleyebilir, silebilir veya
deyimlerin sırasını değiştirebilirsiniz; Komut Dosyası bölmesinin üstündeki kutulara eylemler
için parametreler girebilirsiniz; metni bulup değiştirebilirsiniz ve komut dosyası satır
numaralarını görüntüleyebilirsiniz. Ayrıca bir komut dosyasını iğneleyebilirsiniz; yani,
nesnenin veya karenin dışına tıklattığınızda Komut Dosyası bölmesinde komut dosyasını
tutabilirsiniz.

Komut Dosyası Yardımcısı, acemi bir kullanıcının yapabileceği sözdizimi ve mantık hatalarından
kaçınmanıza yardım eder. Ancak, Komut Dosyası Yardımcısı'nı kullanmak için ActionScript'e
aşina olmanız ve komut dosyalarınızı oluştururken hangi yöntemleri, işlevleri ve değişkenleri
kullanacağınızı bilmeniz gerekir. ActionScript hakkında bilgi edinmek için bkz. Adobe Flash'ta
ActionScript 2.0'ı Öğrenme ve ActionScript 3.0'ı Programlama.


• Değişkeni tanımlamk için "var",

• Değer atamak için de “=” operatörü kullanılır.
var ifade:String="merhaba";

•Değişkene değer atama işlemi değişkeni tanımladıktan sonrada gerçekleştirilir.
var ifade:String;
ifade="Merhaba";

Örnek:1
	// listedeki elmanları for döngüsü ile yazma
	stop();
	var liste:Array=new Array();
	liste[0]="un";
	liste[1]="su";
	liste[2]="meyve suyu";
	for(var i:Number=0; i<liste.length; i++) //listedeki eleman sayısı kadar yaz
	{
		trace(liste[i]);
	}

output ekran çıktısı:
un
su
meyve suyu

Örnek:2

	//Bu fonksiyon bize bir işlem yapıp sonucunu gömrüntülesin
	function fiyatHesapla():Number
	{
		var peynir:Number=7.95;
		var çikolata:Number=1.25;
		var elma:Number=2.50;
		return peynir+elma+çikolata;
	}
	trace("Toplam Fiyatı:"+fiyatHesapla());

output ekran çıktısı:
Toplam Fiyatı:11.7

