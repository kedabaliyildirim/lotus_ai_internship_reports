Orange data mining & Machine Learning udemy kursu bitirildi

Her Seviyeye Uygun Uçtan Uca Veri Bilimi, Knime ile udemy kursu bitirildi

(50 Saat) Python A-Z™: Veri Bilimi ve Machine Learning udemy eğitimi bitirildi

Selenium öğrendim
Öğrendiğim selenium kütüphanesini kullanarak twitter için bir web scrapper oluşturdum
alınan veriler aşağıdaki gibidir:
                    'tweet_text': tweetin kendisi,
                    'replies': tweete verilen cevaplar,
                    'retweets': retweet,
                    'likes': beğeniler,
                    'created_at': oluşturulma tarihi,
                    'username': yazar adı,
                    'following': yazarın takip ettiği kişi sayısı,
                    'followers': yazarı takip eden kişi sayısı,
                    'posts': yazarın attığı iletiler

bunları ile bir dataframe oluşturuldu
basit ön işlemeden geçirldi

twitter web scrapper jupyter notebook tan standart python dosyasına çekildi
kod yeniden düzenlenerek sınıf ve obje mimarisi haline getirildi
kod optimize edildi (9 adet tweet 2 dakikada çekilirken 2-3 saniyede bir tweet çekilebiliyor) 
kod raporu hazırlandı (hangi veri alanları çekiliyor, hangi işlemler uygulanıyor, kod akışı ve yapısı)
knime ile alıştırmalar yapıldı



twitter web scrapper'da olası hataların engellenmesi üzerine çalıştım
env dosyası olmadığı zaman kullanıcıya girdi verilerinin sorulmasını sağladım
KNİME üzerinden 3 adet algoritma ile çalışan (XGB boost, Gradient Boosted Trees, Random Forest) bir model tasarladım 

knime da bir tane output yerine twitter verisinde 3 (likes, retweets, replies) input için 3 er adet model hazırladım  (XGB boost, Gradient Boosted Trees, Random Forest)
metanode yapısını inceledikten sonra sadeleştirmek için metanode'lar kullanıldı
tweeter verisine sentiment analizine başladım (script yazmadan zor gibi duruyor
sql sorularında 15 tane çözüldü (kalan 85)



Flight Delay and Cancellation Dataset (2019-2023) için sınıflandırma görevinin python kısmı tamamlandı kullanılan algoritmalar:
•	KNN
•	XGB
•	LogisticRegression
•	SVM
•	RandomForest
•	NaiveBayes
Star Cluster Simulations için Kümeleme çalışmasının python kısmı tamamlandı kullanılan algoritmalar:
•	K-means
•	Hierarchical
Regresyon ve Birliktelik analizi çalışmalarına başlanıldı


Flight Delay and Cancellation Dataset (2019-2023) için sınıflandırma ve Star Cluster Simulations için kümeleme knime tasarlamasını yaptım
sınıflandırma:
•	XGBoost
•	K nearest
•	Gradient Boosted Tree
Kümeleme:  
•	K-means
•	DBSCAN
Household Electric Power Consumption için regresyon görevini aşağıdaki algoritmaları kullanarak yaptım:
•	Linear Regression
•	Random Forest
•	Gradient Boosting
•	AdaBoost
•	Bagging 
•	naive bayes

•	MLPRegressor
regresyon için knime tasarlaması yaptım:
•	Random Forest
•	Gradient Boosted Tree
Online Retail birliktelik analizinin python kodlarını yazdım.

Online Retail birliktelik analizini için knime tasarımlarını yaptım

Grup içinde paylaşılan pandas sorularını üstüme düşen kısmını knime ortamında oluşturdum

NEREDE TAKILDIM
Kurstaki bazı elementler eskimiş olduğu için knime sistemindeki modern Uİ kullanımından taviz vermem gerekti, bazı noktalarda alternatif Node lar kullanarak çözüm sağladım

Twıtter API kullanımında takıldım, reddit API kullandım 

Selenium yapısından ötürü yavaş çalışan bir sistem zaman kaybına çok sebep oldu, aynı zamanda login işlemleri kalıcı olmadığından ve takipçi sayısı vs bilgileri almak için yeni drivelar oluşturmam gerektiğinden de vakit kaybı oluştu, twitter html kodlarında isimleri XPATH ile ancak güvenilir bir şekilde erişim sağlayabildim

Kodu jupyterden normale geçirmeye karar verdim daha düzgün bir yapısı olması için ancak ne kadar sıkıntılı olabileceğini düşünemediğim için çok vakit kaybına sebep oldu, buna rağmen kodu tekrardan yazmış gibi olduğum için hem hızını arttırdım hemde hata engelleme üzerinde çalışma yapabildim

Knime üzerinde loop yapılarında sıkıntı yaşadım,udemy deki eğitimi tekrar incelediğimde looplar üzerinde çok durulmadığını fark ettim. ek kaynaklardan bakmaya devam etmeyi düşünüyorum

metanode kullanıldığı zaman loop yapıları da metanode içinde olması gerektiğini çok geç anladım, x-partıtıoner ile loop yapısı çakıştığı için sadece basit partition kullanmam gerekti 

Seçtiğim veri setlerinin boyutları 50 100 MB olduğundan ötürü çalışma süreleri çok uzadı, aynı zamanda hiper parametre ayarlaması da bu zaman sınırını kabul edilemeyecek seviyelere taşıdı veri setinden örnekleme yapılarak çözüme ulaşıldı

Knime tarafında modellerin verdikleri hatalar açıklayıcı değil,
bu yüzden python da kullandığım algoritmalardan daha az algoritma kullandımö

support vector makineleri fazla zaman aldığı için algoritmaların 
arasından çıkardım

