---
layout: post
title: Ubuntu Üzerine Adobe Flash 11 Beta Kurmak
---

Güncellenmeyen 64-bit Flash Player eklentisinin yeni sürümü 
çıkartıldı.
Bu yeni sürümde geldiği belirtilen özellikler şu şekilde:

*Stage3D APIs
*64-bit support
*G.711 audio compression for telephony
*H.264/AVC SW Encoding
*Socket Progress Events
*HD surround sound

Eklentinin bu sürümünü kurmak için uçbirimi açarız ve sırası ile aşağıdaki komutları yazarız.

1- <code> sodo apt-add-repository ppa:sevenmachines/flash </code>

<img src="https://github.com/sozgur/sozgur.github.com/blob/master/images/a.png?raw=true" />

2- <code> sudo apt-get update </code>

<img src="https://github.com/sozgur/sozgur.github.com/blob/master/images/b.png?raw=true" />

3- <code>sudo apt-get install flashplugin64-nonfree </code>

<img src="https://github.com/sozgur/sozgur.github.com/blob/master/images/c.png?raw=true" />

Bu güncel sürüm çıktıkça otomatik olarak eklentinin de güncellenmesini sağlayacaktır.

