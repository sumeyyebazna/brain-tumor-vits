# Beyin Tümörü MRI Görüntüleri Üzerinde Vision Transformer Tabanlı Sınıflandırma

Bu projede, beyin tümörü MRI görüntüleri kullanılarak farklı Vision Transformer tabanlı derin öğrenme modelleri eğitilmiş ve karşılaştırılmıştır. Kullanılan modeller:

- ViT (Vision Transformer)
- DeiT (Data-efficient Image Transformer)
- Swin Transformer
- MobileViT
- CvT (Convolutional Vision Transformer)

## Veri Seti

Veri seti, beyin MRI görüntülerinden oluşmaktadır. İki sınıf vardır:
- yes (tümör var)
- no (tümör yok)

Veri seti `train`, `val`, `test` olarak %70-%15-%15 oranında bölünmüştür.

## Kullanılan Modeller

Tüm modeller `timm` kütüphanesi ile önceden ImageNet üzerinde eğitilmiş olarak yüklenmiş ve son katmanları yeniden eğitilmiştir.

## Değerlendirme Ölçütleri

Modeller aşağıdaki ölçütlerle karşılaştırılmıştır:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

## Eğitim Parametreleri

- Batch Size: 8  
- Epoch: 10  
- Optimizer: Adam  
- Learning Rate: 3e-4  
- Loss: CrossEntropyLoss

## Grafikler

Her model için eğitim loss grafiği ve test performans bar grafiği oluşturulmuştur.

## Gerekenler

Tüm gereksinimler için `requirements.txt` dosyasına bakınız.

---

> 📁 Her model için ayrı `.ipynb` dosyası hazırlanmıştır.
> GitHub üzerinden çalıştırılabilir.

