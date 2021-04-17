import requests

adres = "https://pomber.github.io/covid19/timeseries.json"

cevap = requests.get(adres)
veri = cevap.json()

turkiye = veri["Turkey"]

ilk_veri = turkiye[0]

sonVerisayisi = len(turkiye)
sonVeri = turkiye[sonVerisayisi - 1]
#bir gun oncdenin verisi

vakaSayisi = sonVeri["confirmed"]
olumSayisi = sonVeri["deaths"]
iyilesmeSayisi = sonVeri["recovered"]
#keylere ait valuerlerı ata

tarih = sonVeri["date"]
mesaj = "merhaba, {} tarihindeki güncel veri\nvaka saisi:{}\n olum sayisi:{}\niyilesmesayisi:{}\nsaglıklı gunler".format(
    tarih, vakaSayisi, olumSayisi, iyilesmeSayisi)

#son veri diyo aslında ilk veri
#print(ilk_veri)
print(sonVeri)
print(mesaj)
#json formarındaki veriyi ekrana bastık.
