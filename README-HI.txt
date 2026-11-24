RAHUL COMPUTER'S — NEW PROFESSIONAL WEBSITE


फाइलें:
- index.html: नया होमपेज
- services.html: सेवा सूची और श्रेणी फ़िल्टर
- apply.html: ग्राहक आवेदन (Firebase Firestore)
- account.html: ट्रैकिंग नंबर से स्थिति
- admin.html: Admin login और आवेदन स्थिति अपडेट
- privacy.html, terms.html
- assets/style.css, assets/app.js

Firebase project: rahul-computer-s
Firebase Authentication: Admin के लिए पहले से बना Email/Password account उपयोग करें। Admin UID allowlist: Fe7XhLLbCGdJ0d9KtqSkqiCNTQG3

महत्वपूर्ण सेटअप:
1) Firebase Hosting पर इस फ़ोल्डर को deploy करें।
2) Firestore Rules में applications पर public create के लिए पुराने नियम पहले से अनुमति देते हों तभी आवेदन सीधे सेव होगा। इस साइट में कोई permissive security rules स्वतः नहीं जोड़े गए हैं।
3) tracking collection में public get/create rules की अनुमति हो तभी tracking lookup काम करेगा। यदि rules रोकें, apply form WhatsApp fallback दिखाता है।
4) Admin read/update के लिए मौजूदा UID-based rules आवश्यक हैं।
5) Firebase Console > Authentication में Email/Password provider enabled होना चाहिए।
6) इस पोर्टल में वास्तविक सरकारी API integration शामिल नहीं है। प्रत्येक सरकारी सेवा अधिकृत API/official portal access मिलने पर ही automate की जा सकती है।
7) सार्वजनिक लॉन्च से पहले Firestore Rules, App Check, abuse protection, privacy notice और form behavior की जाँच करें।

यह ZIP static frontend है। इसे तैयार/पैकेज किया गया है; Hosting पर deploy या live Firebase integration test नहीं किया गया।
