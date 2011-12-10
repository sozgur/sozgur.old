---
layout: post
title: ActionScript Nedir?
---

ActionScript, Flash Player için oluşturulan içeriklere etkileşim kazandırmak için kullanılan
programlama dilidir.

ActionScript programlama dili Flash ve Flex programları ile kullanılmaktadır. Bu dil ile
etkileşimli, sonrasında update edilip geliştirilebilen uygulamalar geliştirmek mümkündür.

ActionScript ile yapılacak bazı işlemlere kısaca göz atacak olursak;
<p>-Fare ya da klavye olaylarına yanıt verilebilir,</p>
<p>• click event yani fare ile tıklama, tuşa basılması veya dosya yüklemesidir.</p>
<p>-Harici dosyalarla çalışılabilir (Ses, görsel, metin, video),</p>
<p>-Çizim ya da boyama yapılabilir,</p>
<p>-Yapılan uygulamaların yazıcılardan çıktısının alınması sağlanabilir,</p>
<p>-Matematik ya da Fizik hesaplamaları yaptırılabilir,</p>
<p>-Animasyonlar hazırlanabilir.</p>

ActionScript kullanarak uygulamaları doğrusal olmayan bir şekilde oynatabilir ve uygulamalara
zaman çizelgesinde temsil edilemeyen ilginç veya karmaşık işlevler eklenilebilir.

ActionScript kodlama dili uygulamalara karmaşık etkileşimler, oynatma kontrolü ve veri
görüntüleri eklemeyi sağlar.

ActionScript kendi sözdizimi kurallarına, ayrılmış anahtar sözcüklerine uyar ve bilgi depolamak
ve geri almak için değişkenlerin kullanılmasını sağlar. ActionScript birçok faydalı görevin
gerçekleştirilmesini sağlayan nesneler oluşturmasına izin veren, yerleşik sınıflardan oluşan
geniş bir kitaplık içerir.

Örnegin:
<p>import flash.display.*;</p>

Eylemler panelini, Komut Dosyası penceresini veya harici bir düzenleyiciyi kullanarak geliştirme
ortamına ActionScript eklenilebilir.

Örnek:

	package
	{
		import flash.display.*;
		public class deneme extends MovieClip
		{
			public function deneme()
			{
				trace("kod çalışıyor")
			}
		}

şeklinde bir kod yazdık ve bunu deneme.as olarak kaydetdik. Sayfayı kaydettikten sonra bu
işlemi test edebilmek için bu ActionScript dosyasını bir MovieClip'e bağlıyoruz.

	package
	{
		import flash.display.*;
		import flash.event.*;
		public class deneme extends MovieClip
		{
			puplic function deneme()
			{
				this.addEventListener(MouseEvent.MOUSE_DOWN, basla);
				this.addEventListener(MouseEvent.MOUSE_DOWN, bitir);
			}
			public function basla(event:MouseEvent): void
			{
				this.startDrag();
			}
			public function biti(event:MouseEvent): void
			{
				this.stopDrag();
			}
		}
	}


<p>Package: içerisinde classları tutar packace paketAdı.</p>
<p>{</p>
<p>classlarla ilgili kodlar burya gelecek</p>
<p>{</p>

örn:

<p>Packace Canlılar</p>
<p>{</p>
<p>puplic class Papatya</p>
<p>{</p>

ActionScript ve JavaScript, köklerini ECMAScript kodlama dilinin uluslararası standardı olan
ECMA-262 standardından alırlar.



ActionScript sürümleri

Flash, farklı türdeki geliştiricilerin ve oynatma donanımının ihtiyaçlarını karşılamak amacıyla
birden fazla ActionScript sürümü içerir.

- ActionScript 3.0 son derece hızlıdır. Bu sürüm, nesneye yönelik programlama kavramına diğer
ActionScript sürümlerinden biraz daha fazla aşinalık gerektirir. ActionScript 3.0 ECMAScript
tanımlamasıyla tamamen uyumludur, daha iyi XML işleme, iyileştirilmiş bir olay modeli ve
ekrandaki öğelerle çalışmak için iyileştirilmiş bir mimari sunar. ActionScript 3.0 kullanan
dosyalar ActionScript'in önceki sürümlerini içeremezler.

- ActionScript 2.0'yi öğrenmek ActionScript 3.0'ü öğrenmekten daha kolaydır. Flash Player
derlenmiş ActionScript 2.0 kodunu derlenmiş ActionScript 3.0 kodundan daha yavaş çalıştırsa
da, daha tasarıma dayalı içerikler gibi ActionScript 2.0 hesaplama açısından yoğun olmayan
birçok türde proje için kullanışlıdır. ActionScript 2.0 de ECMAScript tabanlıdır ancak tamamen
uyumlu değildir.

- ActionScript 1.0, ActionScript'in en basit halidir ve Flash Lite Player'ın bazı sürümleri
tarafından hala kullanılmaktadır. ActionScript 1.0 ve 2.0, aynı FLA dosyası içinde bir arada
bulunabilirler.

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

kodun output ekranındaki çıktısı:</p>
<p>Alınacaklar listesi</p>
<p>1-Deterjan</p>
<p>2-Peyneri</p>
<p>3-Süt</p>
<p>4-Çay</p>

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


<p>• Değişkeni tanımlamk için "var",</p>

<p>• Değer atamak için de “=” operatörü kullanılır.</p>
<p>var ifade:String="merhaba";</p>

<p>•Değişkene değer atama işlemi değişkeni tanımladıktan sonrada gerçekleştirilir.</p>
<p>var ifade:String;</p>
<p>ifade="Merhaba";</p>

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

<p>output ekran çıktısı:</p>
<p>un</p>
<p>su</p>
<p>meyve suyu</p>

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

<p>output ekran çıktısı:</p>
<p>Toplam Fiyatı:11.7</p>



