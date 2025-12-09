Selahattin Düyme
---

# 📌 NetBeans Java Öğrenci Tablosu Yönetimi

Bu proje, **Java Swing** ve **NetBeans** kullanılarak hazırlanmış basit bir öğrenci tablosu yönetim uygulamasıdır.
Kullanıcı arayüzü üzerinden listeye öğrenci ekleme ve seçili öğrenciyi silme işlemleri yapılabilir.

---

## 🔧 Kullanılan Teknolojiler

* Java (Swing)
* NetBeans IDE
* DefaultListModel
* JList, JButton, JTextField bileşenleri

---

## 🎯 Özellikler

* Öğrenci ekleme
* Seçili öğrenciyi kaldırma
* Liste üzerinde dinamik güncellemeler
* Hatalı seçim kontrolü

---

## 📁 Proje Yapısı

```
src/
nbproject/
build/
build.xml
manifest.mf
README.md
```

---

## ▶️ Çalıştırma

1. NetBeans’i açın
2. `File > Open Project` ile bu projeyi seçin
3. `Run Project (F6)` tuşu ile çalıştırın

---

## 📝 Örnek Kod – Silme İşlemi

```java
int index = lstOgr.getSelectedIndex();

if(index != -1) {
    String silinen = model.getElementAt(index).toString();
    model.removeElementAt(index);
    lblSonuc.setText("Seçili öğrenci silindi: " + silinen);
} else {
    lblSonuc.setText("Öğrenci seçimi yapılmadı!");
}
```

---

## 📌 Amaç

Java Swing ile GUI geliştirmeye yeni başlayanlar için temel bir liste yönetimi örneği sunar.

---
