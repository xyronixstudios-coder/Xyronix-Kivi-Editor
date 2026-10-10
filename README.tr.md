# 🥝 Xyronix Kivi Editor

> Go ile yazılmış modern, modeless (modsuz) terminal metin editörü.
> **Eren Mut** tarafından · [Xyronix Studios](https://github.com/xyronixstudios-coder)

[![Lisans: GPL v2](https://img.shields.io/badge/Lisans-GPL%20v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
[![Go Sürümü](https://img.shields.io/badge/Go-1.20%2B-00ADD8.svg)](https://go.dev/)
[![Derleme Durumu](https://github.com/xyronixstudios-coder/Xyronix-Kivi-Editor/actions/workflows/build.yml/badge.svg)](https://github.com/xyronixstudios-coder/Xyronix-Kivi-Editor/actions)

[🇬🇧 For English, click here](README.md)

---

## 📖 İçindekiler

- [Kivi Nedir?](#-kivi-nedir)
- [Özellikler](#-özellikler)
- [Ekran Görüntüleri](#-ekran-görüntüleri)
- [Kurulum](#-kurulum)
- [Kullanım](#-kullanım)
- [Klavye Kısayolları](#️-klavye-kısayolları)
- [Fare Desteği](#️-fare-desteği)
- [Yapılandırma](#️-yapılandırma)
- [Kaynaktan Derleme](#-kaynaktan-derleme)
- [Mimari](#️-mimari)
- [Katkıda Bulunma](#-katkıda-bulunma)
- [Lisans](#-lisans)
- [Emeği Geçenler](#-emeği-geçenler)

---

## 🥝 Kivi Nedir?

**Xyronix Kivi Editor** (kısaca: **kivi**), GNU nano'dan esinlenmiş ama
2026 için modernize edilmiş hafif, **modsuz** bir terminal metin
editörüdür.

**vi/vim**'in aksine kivi **modsuzdur**: her basılabilir tuş anında
metne yazılır, komutlar sadece `Ctrl` kombinasyonlarındadır. `hjkl`
yok, `:wq` yok, `Esc`'e basıp moddan çıkmak yok, gizli mod yok.
Editörü açar ve yazmaya başlarsın — bu kadar.

**nano**'dan farkları:

- Modern **kivi-yeşili** renk teması, koyu terminallerde okunaklı
- Gerçek **fare desteği**: tıkla → imleç oraya, sürükle → metin seç,
  tekerlek → kaydır, bırakınca otomatik kopyala (OSC 52)
- **UTF-8** doğal destek, çoklu dil (Türkçe, Çince, Arapça, Kiril,
  Devanagari, ...)
- Terminal pencereni büyütüp küçültünce **anında yeniden çizim**
  (SIGWINCH)
- [bubbletea](https://github.com/charmbracelet/bubbletea) ve
  [lipgloss](https://github.com/charmbracelet/lipgloss) ile temiz
  **Go** kod tabanı

Kivi, hızlı bir düzenleme, config değişikliği ya da script yazmak
için açtığın editördür — nano'nun yerini alır ama modern hissiyatla.

---

## ✨ Özellikler

| Kategori | Özellik |
|----------|---------|
| **Düzenleme** | Modsuz, hjkl yok, insert mode yok |
| **Girdi** | Tam UTF-8, CJK geniş karakter (genişlik = 2) |
| **Fare** | Tıkla, sürükle-seç, tekerlek kaydır, otomatik kopyala (OSC 52) |
| **Görünüm** | Kivi-yeşili tema, satır numaraları, tilde, durum çubuğu |
| **Boyut** | Terminal yeniden boyutlandırılınca canlı çizim (SIGWINCH) |
| **Tuşlar** | Nano uyumlu: `^O`, `^X`, `^W`, `^K`, `^U`, `^A`, `^E`, `^Y`, `^V`, `^G`, `^R`, `^C` |
| **G/Ç** | Aç, kaydet, farklı kaydet, kaydetme uyarısıyla çık |
| **Arama** | İleri arama, başa sarma (`^W`) |
| **Kesme** | Satır cut buffer, çok satırlı kesme, yapıştırma (`^K` / `^U`) |
| **Çoklu dil** | Türkçe, İngilizce, Arapça, Çince, Kiril ve daha fazlası |

---

## 📸 Ekran Görüntüleri

> _Ekran görüntüleri yakında. kivi çalışırken ekran görüntüsü al ve PR gönder!_

---

## 🚀 Kurulum

### Hızlı kurulum (her dağıtım)

```bash
git clone git@github.com:xyronixstudios-coder/Xyronix-Kivi-Editor.git
cd Xyronix-Kivi-Editor
./install.sh
