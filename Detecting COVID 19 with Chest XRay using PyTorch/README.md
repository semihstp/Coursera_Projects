[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/semihstp/Coursea_Projects/blob/main/Detecting%20COVID%2019%20with%20Chest%20XRay%20using%20PyTorch/Detecting_COVID_19_with_Chest_X_Ray_using_PyTorch.ipynb)

Bu proje Coursea'nın [Detecting COVID-19 with Chest X-Ray using PyTorch](https://www.coursera.org/projects/covid-19-detection-x-ray) projesidir.

# Dataset

Kaggle platformundaki [COVID-19 Radiography Database](https://www.kaggle.com/tawsifurrahman/covid19-radiography-database) veri seti kullanılmıştır. 'Normal', 'Covid' ve 'Viral Pneumonia' olmak üzere 3 sınıfa sahiptir. 3616 COVID, 10192 normal ve 1345 Viral Pneumonia röntgenlerinden oluşan veri seti Kaggle üzerinden sürekli güncellenmekle birlikte dördüncü bir sınıf olarak akciğer kanseri de eklenmiştir. Ancak gerçekleştirilen çalışmada sadece üç sınıfa yer verilmiştir.

## Model
Çalışmada PyTorch kütüphanesi kullanılmıştır. Backbone olarak Resnet18 mimarisi alınmıştır. Bazı önemli parametreler:

| Image Size | Batch_size | Epoch |in_features | out_features | learning_rate |
| :---: | :---: | :---: | :---: | :---: | :---: |
| (244, 244) | 6 | 1 | 512 | 3 | 3e-5 |

## Örnek Çıktılar

Eğitimin ilk aşamalarında elde edilen sonuçlar :

* Evaluating at step 20:
![step_20](https://user-images.githubusercontent.com/56072259/126179726-1512f6dc-2eaf-4d16-ae08-0e1246f344de.png)

```Validation Loss: 0.9850, Accuracy: 0.5444```

* Evaluating at step 200 (acc>95'e geldiği an eğitim sonlandırılmıştı.) :
![step_20](https://user-images.githubusercontent.com/56072259/126179715-c5789584-15c0-4fb8-be4b-6de9c970030b.png)

## Benimle iletişime geçin!
[![](https://user-images.githubusercontent.com/56072259/121079707-28be5d00-c7e3-11eb-9666-9acb3dd9526a.png)](https://www.linkedin.com/in/semih-gulum/)
[![](https://user-images.githubusercontent.com/56072259/121079953-7c30ab00-c7e3-11eb-8e4d-506fabc530a5.png)](mailto:sgulum98@gmail.com)
[![](https://user-images.githubusercontent.com/56072259/121080373-0416b500-c7e4-11eb-833c-e6abe08efea0.png)](https://semihstp.github.io/)
