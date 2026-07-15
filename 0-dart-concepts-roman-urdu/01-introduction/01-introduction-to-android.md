# Android — Introduction

## Android Kya Hai?
Android ek **Operating System (OS)** hai jo khaas tor par mobile
devices ke liye banaya gaya hai. Jaise computer ko chalane ke liye
Windows jaisi OS chahiye hoti hai, waise hi mobile ka hardware —
**screen, camera, battery, sensors** — sab kuch control aur coordinate
karne ke liye ek operating system chahiye hoti hai. Wahi operating
system **Android** hai.

> **Android → Mobile Devices Ka Operating System**

---

## Android Kyun Khaas Hai — Open Source
Android ka sab se bada faida ye hai ke ye **Open Source** hai. Matlab
Google ne iska underlying source code **sabke liye free** rakha hai.
Isi openness ki wajah se **Samsung, Oppo, Vivo, aur Xiaomi** jaisi
companies Android ka wahi core code lekar, upar ka visual layer
(**UI** — User Interface) apne hisaab se badal leti hain, aur apne
naam se brand kar deti hain (jaise Samsung ka "One UI", Xiaomi ka
"MIUI").

Simple lafzon mein: Android ka jo base code hai wo in sab companies ke
pass **same** hota hai. Har company sirf **UI/UX layer** ko upar se
customize karti hai — lekin core functionality, kernel, aur system
architecture wahi Android ka foundation rehta hai.

> Yehi wajah hai ke tumhara Samsung phone aur tumhare dost ka Xiaomi
> phone "feel" mein alag lagte hain, lekin dono par Android apps
> bilkul theek chalti hain.

---

## Lafz "Android" Kahan Se Aaya
"Android" lafz **Greek** zuban se aaya hai, jiska matlab hai **"insaan
jaisa"** ya **"insaan se milta julta"**:

- **andr-** → mard / insaan
- **-oeidēs** → jaisa / milta julta

Purane science-fiction mein "android" ek aise robot ke liye use hota
tha jo dikhne mein insaan jaisa ho — Google ne apni mobile OS ke liye
yehi naam le liya.

> **Technical definition:** Android ek **Linux-based, open-source
> operating system** hai jo Google ne banayi, khaas tor par
> touchscreen mobile devices jaise smartphones aur tablets ke liye.

---

## Zaroori Alfaaz (Key Terms)

| Term | Matlab |
|------|--------|
| **Android** | Mobile device ka "dimaag" (Operating System) |
| **Google** | Wo company jo Android ki malik hai aur ise develop karti hai |
| **Flutter** | Ek framework/tool jisse Dart language use karke Android (aur doosre platforms) ke liye apps banayi jati hain |
| **Play Store** | Google ki official dukaan jahan se Android apps distribute aur download hoti hain |
| **Kernel** | Android ka core hissa (Linux kernel par based) jo hardware resources manage karta hai |

---

## Android Versions aur API Levels
Tumne shayad suna hoga **"Android 12"**, **"Android 13"**, ya
**"Android 14"** — ye Android ke **public version names** hain.

Lekin coding ki duniya mein, har Android version ko ek numeric
**API Level** bhi diya jata hai. Jab developers app banate hain, to
unhe apni app ka **minimum API Level** batana padta hai — is se system
ko pata chalta hai ke app kis se kis purane Android version tak
compatible hai.

> **Misal:** "Ye app Android 5.0 aur uske baad chalti hai" ka matlab
> hai ke app ka `minSdkVersion` us API Level par set hai jo Android 5.0
> (API Level 21) ke barabar hai.

| Android Version | API Level |
|------------------|----------------------|
| Android 5  | 21 |
| Android 10 | 29 |
| Android 12 | 31 |
| Android 13 | 33 |
| Android 14 | 34 |

> **Android Version → API Level** (dono ek doosre se directly juray
> hote hain, aur zyada API Level ka matlab hai naye system features
> tak access)

---

## Quick Recap
> - **Android** = Mobile ki Operating System, **Google** ne banayi
> - **Open Source** → companies shared core code par apni UI customize
>   kar sakti hain
> - Naam **Greek** se aaya, matlab "insaan jaisa"
> - **Linux-based** system hai
> - Har version ka apna **API Level** hota hai, jo developers app
>   compatibility set karne ke liye use karte hain
