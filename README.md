
# Sınıflandırma modellerinin performansını değerlendirmede ROC-AUC’u

Arkadaşlar tekrar merhaba. Daha önceki yazılarımla da ilgili olması açısından önemli bir konu olduğunu düşündüğüm model performans değerlendirilmesi ile alakalı bir yazı  kaleme almak istedim.

Bir sınıflandırma problemi için geliştirilen modelin performansı  genel olarak F1 Score, Recall, Accuracy, Precision, Confusion Matrix gibi metriklerle ölçülse de bu çalışmada ROC - AUC eğrisi üzerine odaklanacağız. Bu metrik, çeşitli eşik ayarlarında sınıflandırma problemleri için bir performans ölçümüdür. 

ROC bir olasılık eğrisidir ve AUC ayrılabilirlik derecesini veya ölçüsünü temsil eder. Daha geniş bir ifadeyle bu eğri, modelin sınıfları ne kadar ayırt edebildiğini gösterir. AUC ne kadar yüksekse, model doğru tahminlerde o kadar başarılıdır denebilir. 

Şekil üzerinde inceleyelim.

![image](https://github.com/tr-brain-com/roc-auc/assets/118043046/829c40ff-d3b5-4e9a-94b5-9dfbb55bcebb)

ROC (Area Under Curve)

AOC (Receiver Operating Characteristics)

TPR (True Positive Rate)

FPR (False Positive Rate)


ROC eğrisi, TPR'nin y ekseninde ve FPR'nin x ekseninde olduğu FPR'ye karşı TPR ile çizilir. Kısaca TPR ve FPR nin hesaplanmasına da değinelim.

# Toplam Doğru Oranının Hesaplanması
![image](https://github.com/tr-brain-com/roc-auc/assets/118043046/f9f91a02-9cb1-45de-a8d0-4f830f0d1357)

# Toplam Yanlış Oranının  Hesaplanması
![image](https://github.com/tr-brain-com/roc-auc/assets/118043046/45037148-4005-4f77-8887-4599de738b78)

**Sensitivity:** Modelin pozitif sonuçları “pozitif” olarak tahmin etme durumudur. Literatürde Gerçek Pozitif Oran (true positive rate)" da denir.

**Specificity:** Modelin negative sonuçları “negative” olarak tahmin etme durumudur. Literatürde Gerçek Pozitif Oran (true negative rate)" da denir.

Yazı serisinin tamamını okumak için [tıklayınız](https://www.brain-tr.com/classification-modellerinin-performansini-degerlendirmede-roc-auc/).

Notebook dosyası için [tıklayınız](https://github.com/tr-brain-com/roc-auc/blob/main/roc_auc_app.ipynb).
