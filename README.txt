HISAAB APP - APK BANANE KI GUIDE (zero budget)
==============================================

Is zip mein poora project hai. Tumhein bas ise GitHub par daalna hai,
baqi kaam GitHub khud karega aur APK bana dega.

STEP 1: GitHub account
  github.com par free account banao.

STEP 2: Naya repository
  "New repository" dabao, naam hisaab-app rakho, Create dabao.

STEP 3: Files upload karo
  Zip ko apne phone ya laptop mein khol (extract) lo.
  Repository mein "uploading an existing file" ya "Add file > Upload files" dabao.
  Zip ke ANDAR ki saari files aur folders (www, resources, package.json,
  package-lock.json, capacitor.config.json, .gitignore, README.txt) drag karke upload karo, phir "Commit changes" dabao.

STEP 4: Build wali file (.github folder)
  Kuch phones/computers hidden folder (.github) upload nahi karte.
  Agar repository mein .github/workflows/build.yml nazar na aaye to:
    - "Add file > Create new file" dabao
    - Naam ki jagah yeh likho:  .github/workflows/build.yml
      (slash likhte hi folder khud ban jata hai)
    - github-workflow-build.yml.txt ka poora matn copy karke wahan paste karo
    - "Commit changes" dabao.

STEP 5: APK ka intezar
  Repository ke upar "Actions" tab kholo. "Build APK" chalta nazar aayega.
  Isay 5 se 10 minute lag sakte hain. Hara tick aa jaye to build tayyar hai.
  Agar laal X aaye to us par click karke error ka matn mujhe bhej do.

STEP 6: APK download
  Hare tick wale run par click karo, neeche "Artifacts" mein "hisaab-apk"
  download karo. Wo ek zip hoga, usay khol kar app-debug.apk nikalo.

STEP 7: Phone mein install
  APK ko phone mein bhejo, kholo, "Install unknown apps" ki ijazat do, install karo.

NOTES
  - App offline chalti hai. Tumhara hisaab phone mein hi save hota hai.
  - PDF button dabane par share/save ki list khulti hai (Drive, Files, WhatsApp wagaira).
  - Mic button Android app mein aam taur par nahi chalta, isliye chhup jata hai.
  - Yeh debug APK hai: apne phone aur doston ke liye theek hai.
    Play Store ke liye signed AAB aur $25 developer fee chahiye.
  - App ka apna icon (gradient par kagaz-hisaab ka nishan) resources/res folder
    mein hai, workflow usay khud lagata hai. Folder delete mat karna.
  - Status bar ka masla theek kar diya hai: app ab status bar aur neeche wali
    navigation bar ke neeche nahi chhupti (capacitor.config.json mein
    adjustMarginsForEdgeToEdge = force). Dark mode mein status bar ka rang
    halka jamni rehta hai.
  - Agar phir bhi koi masla aaye to screenshot bhej do.
