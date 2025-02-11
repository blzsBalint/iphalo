# Jegyzőkönyv: Hálózati konfiguráció és tesztelés

## Bevezetés

Ez a jegyzőkönyv a Linksys router beállítását és a hozzá kapcsolódó hálózati eszközök tesztelését dokumentálja. A feladat során IP-címek kezelése, routing tábla megtekintése, ping tesztek és egyéb hálózati parancsok alkalmazása történt.




## Eszközök
A tesztelés során a következő eszközökkel dolgoztam:
- **Catalyst 2950 switch**: A hálózati eszközök közötti kapcsolatot biztosította.
- **Linksys router**: A hálózat központi irányítószerveként szerepelt.
- **ThinkPad laptop**: A teszteléshez használt számítógép, amelyről a ping tesztek és egyéb parancsok futtak.
- **Mobiltelefon**: Ezzel csatlakoztam a Linksys routerhez, hogy a laptop és a többi eszköz között pingelni tudjak.
## 1. A számítógép IP beállításainak lekérdezése
Parancs: `ipconfig`
<details>
  <summary>Kép megtekintése</summary>


  !
</details>

## 2. Az aktuális IP-cím eldobása
Parancs: `ipconfig /release`
<details>

  <summary>Kép megtekintése</summary>
![02 11 release](https://github.com/user-attachments/assets/77ba413e-a881-4ada-b5f9-8de8ae419b2d)

 
</details>

## 3. Új IP-cím kérése
Parancs: `ipconfig /renew`
<details>

  <summary>Kép megtekintése</summary>

  ![02 11 lock](https://github.com/user-attachments/assets/7ba761cd-56c8-40f3-baef-7fd19fca79b6)


</details>

## 4. A routing tábla megjelenítése
Parancs: `netstat -a`
<details>

  <summary>Kép megtekintése</summary>

![02 11 netstat](https://github.com/user-attachments/assets/dc7177e0-e707-4963-b0a1-1c366f0ff009)


</details>


  <summary>Kép megtekintése</summary>

 ![02 11 microsoft](https://github.com/user-attachments/assets/c384538f-cd25-4966-8f1a-83ab2e86b708)


</details>

## 6. Az www.ipon.hu szerver felé vezető útvonal lekövetése
Parancs: `tracert www.ipon.hu`
<details>

  <summary>Kép megtekintése</summary>
 ![02 11 ipon](https://github.com/user-attachments/assets/77b5f92a-e1b5-4794-8893-b503ad19504e)


 
</details>

## 7. Használt portok listázása
Parancs: `netstat -f`
<details>

  <summary>Kép megtekintése</summary>

  ![02 11 f](https://github.com/user-attachments/assets/ce91ffe1-bc6c-445b-b68d-ce4b60fc2068)


</details>

## 8. Hálózati kapcsolatok megjelenítése
Parancs: `netsh interface show interface`
<details>

  <summary>Kép megtekintése</summary>

  ![02 11 netsh](https://github.com/user-attachments/assets/a1873ba8-e204-4f24-b751-f5312bbe36c6)


</details>

## 9. DNS-beállítások aktualizálása
Parancs: `ipconfig /flushdns`
<details>

  <summary>Kép megtekintése</summary>

  ![flushdns](https://github.com/PavlyasB/IPhalo/blob/main/Képek/dnsflush.png?raw=true)

</details>

## 10. Csatolt hálózati meghajtók megjelenítése
Parancs: `net use`
<details>

  <summary>Kép megtekintése</summary>

  ![netuse](https://github.com/PavlyasB/IPhalo/blob/main/Képek/netuse.png?raw=true)

</details>

## 11. A www.ipon.hu tartománynév és IP-cím megjelenítése
Parancs: `nslookup www.ipon.hu`
<details>

  <summary>Kép megtekintése</summary>

  ![02 11  ipon slukk](https://github.com/user-attachments/assets/a5d7b942-c636-4b5b-a2f0-ae9e6db42379)


</details>

## 12. Telefon rákapcsolódva a Wi-Fi-re
<details>
  <summary>Kép megtekintése</summary>
![telefon 1](https://github.com/user-attachments/assets/3278cc35-ad54-4a01-ba18-b95b812b4e53)
![telefon 2](https://github.com/user-attachments/assets/9e89d57f-897f-44ba-85be-cfab35cc60cf)

 
</details>

## 13. Telefon pingelése laptopról
<details>
  <summary>Kép megtekintése</summary>
![02 11 telefon ping](https://github.com/user-attachments/assets/c450e334-1ddb-4ff4-878d-204d7fcb9610)

  
</details>

## 14. Router konfigurációk
<details>
  <summary>Kép megtekintése</summary>
![02 11 ssid](https://github.com/user-attachments/assets/5ee7a158-5790-40fc-b8d3-ca4ab483f64f)

 
</details>

<details>
  <summary>Kép megtekintése</summary>

  ![02 11 setup](https://github.com/user-attachments/assets/d9e39612-0ca8-4892-9159-6b34d077d600)

</details>
![02 11 lock](https://github.com/user-attachments/assets/3e0016a6-b014-4b27-b9e9-a00df428e808)

<details>

  <summary>Kép megtekintése</summary>

  
</details>

## Összegzés
A tesztelés során a **Linksys router**, a **Catalyst 2950 switch** és a többi hálózati eszköz zökkenőmentesen működtek együtt. Az IP-konfigurációk kezelése, a routing tábla megjelenítése és a különböző hálózati parancsok futtatása sikeresen zajlott. A mobiltelefonnal való csatlakozás lehetővé tette a laptop és a többi eszköz közötti kommunikációt.
