---
layout: post
title: ActionScript Nedir?
---

ActionScript, Flash Player için oluşturulan içeriklere etkileşim kazandırmak için kullanılan
programlama dilidir.

ActionScript programlama dili Flash ve Flex programları ile kullanılmaktadır. Bu dil ile
etkileşimli, sonrasında update edilip geliştirilebilen uygulamalar geliştirmek mümkündür.

ActionScript ile yapılacak bazı işlemlere kısaca göz atacak olursak;
-Fare ya da klavye olaylarına yanıt verilebilir,
 • click event yani fare ile tıklama, tuşa basılması veya dosya yüklemesidir.
-Harici dosyalarla çalışılabilir (Ses, görsel, metin, video),
-Çizim ya da boyama yapılabilir,
-Yapılan uygulamaların yazıcılardan çıktısının alınması sağlanabilir,
-Matematik ya da Fizik hesaplamaları yaptırılabilir,
-Animasyonlar hazırlanabilir.

ActionScript kullanarak uygulamaları doğrusal olmayan bir şekilde oynatabilir ve uygulamalara
zaman çizelgesinde temsil edilemeyen ilginç veya karmaşık işlevler eklenilebilir.

ActionScript kodlama dili uygulamalara karmaşık etkileşimler, oynatma kontrolü ve veri
görüntüleri eklemeyi sağlar.

ActionScript kendi sözdizimi kurallarına, ayrılmış anahtar sözcüklerine uyar ve bilgi depolamak
ve geri almak için değişkenlerin kullanılmasını sağlar. ActionScript birçok faydalı görevin
gerçekleştirilmesini sağlayan nesneler oluşturmasına izin veren, yerleşik sınıflardan oluşan
geniş bir kitaplık içerir.

Örnegin:
import flash.display.*;

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
			public function basla(event:MouseEvent):void
			{
				this.startDrag();
			}
			public function biti(event:MouseEvent):void
			{
				this.stopDrag();
			}
		}
	}


Package: içerisinde classları tutar packace paketAdı.
{
classlarla ilgili kodlar burya gelecek
{

örn:

Packace Canlılar
{
puplic class Papatya
{

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


