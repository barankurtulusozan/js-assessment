[![Build Status](https://travis-ci.org/rmurphey/js-assessment.svg?branch=master)](https://travis-ci.org/rmurphey/js-assessment)

# Test Güdümlü JavaScript Geliştirme Egzersizleri

Bu repo kişilerin JavaScript yeteneklerini ölçerken, geliştirmelerine de yardımcı olmaktadır.

Not: [Nasıl çalıştırırım?](https://blog.bko.io/index.php/2017/08/09/javascript-bilginizi-test-edin/)

Not2: [Bu reponun sahibi Rebecca Murphy'nin Disqus'tan Burak Yiğit Kaya (madbyk) ile TTL röportajı - As bayrakları edition](http://ttlpodcast.com/episodes/burak-yigit-kaya.html)

## Testlerle çalışmak için ne yapmalıyım?
Öncelikle bilgisayarınızda Node kurulu olmalı, değilse bu adresten indirin [Node](https://nodejs.org/) . Windows işletim sistemli bilgisayarlarda Node yüklendikten sonra bazen yeniden başlatılması gerekmektedir. Bkz #12.

Bu repoyu indirebilir veya klonlayabilirsiniz. Bunu yaptıktan sonra kök dizinine giderek (egzersizleri indirdiğiniz klasöre node komut ekranından erişmek için cd klasörAdi komutunu kullanın), egzersiz klasörünün bulunduğu dizinde aşağıdaki komutları çalıştırın.
    npm install
    npm start

Tarayıcınızda testleri aşağıdaki adreste görüntüleyebilirsiniz.
[http://localhost:4444](http://localhost:4444).

Sayfa açıldığında bütün testlerin başarısız olduklarını göreceksiniz. Göreviniz 
kırmızı çarpı'ları yeşil tiklere dönüştürmek. Bunun için projeyi favori editörünüzle
açtıktan sonra (Sublime/Atom/Notepad++/Emacs vb.) 'tests/app' klasöründe yer alan
test fonksiyonlarının içlerini doğru şekilde doldurmalısınız. (parametre 
isimlendirmelerine dikkat edin) Her save/sakla/kaydet dediğinizde tarayıcınızdaki
 testin yeniden yüklenerek kontrol edildiğini göreceksiniz. Sayfa yenilemenize gerek
yoktur. Testlerin çoğunu komut satırından çalıştırabilirsiniz.

    npm test

Komut satırı yorumlayıcısı hala geliştirilmektedir, destekleriniz memnuniyetle karşılanacaktır.

### Mevcut Bağımlılıklar

Bu repoda jQuery, Backbone ve Underscore 3.parti bağımlıkları yer almaktadır.Kendi 
çözümleriniz için bunlardan faydalanabilirsiniz..

## Katkıda bulunmak istiyorum, ne yapmalıyım?

Pull request talbeinde bulunun. Testler konu başlıklarına göre şu anda geniş geniş
sınıflandırılmış durumda, bu sebeple `tests/app` içinde uygun yere ekleme yaparken 
elinizden geleni ardınıza koymayın, eğer uygun bir seçenek göremezseniz yeni bir dosya
oluşturun, eğer yeni bir dosya oluşturursanız `tests/runner.js`onu buraya eklemeyi 
unutmayın. Son olarak eğer [çözümler](https://github.com/rmurphey/js-assessment-answers)'i
de linkteki adrese eklerseniz iyi olur.

Eğer testi nereye ve nasıl ekleyeceğinizden emin değilseniz lütfen bir issue açın.

### Data-driven tests

If your tests need data that can be fetched via XHR, stick a `.json` file in
the `data` directory; you can access it at `/data/<filename>.json`.

## I want to see the answers!

First, bear in mind that looking up the answers is going to teach you a whole
lot less than you'll learn by working on the tests, even if you occasionally get
stuck. I'd recommend only looking at the answers once you have the tests
passing, to see if there's another way you could have approached the
problem. When you're ready to look at the answers, you can find them
[here](https://github.com/rmurphey/js-assessment-answers); I'll do my best to
keep them up to date.

## I hate \<some technology you've chosen\>

This repo uses [Mocha](https://github.com/mochajs/mocha) and
[Chai](http://chaijs.com/) for the tests themselves. It uses the BDD style for authoring tests.
If this doesn't suit you, please fork away, or, better, submit a pull request that lets
this be more flexible than it currently is.

# Todos

There are a number of things that would make this project better; check out the
[issues](https://github.com/rmurphey/js-assessment/issues) for details, pull
requests welcome!

# License

Copyright &copy; 2012-2016 Rebecca Murphey with many thanks to several
[contributors](https://github.com/rmurphey/js-assessment/graphs/contributors).

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
