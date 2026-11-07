KhetDristi - Hosting Guide
==========================
Ye ek single-page static site hai. Koi server, database ya build step nahi chahiye.
Sab kuch index.html ke andar hai.

Files:
  index.html   -> poora prototype (isko root mein rakhna hai)
  README.txt   -> ye guide

Hosting (koi bhi ek):
  1) Netlify  : app.netlify.com/drop -> poora folder (unzip karke) drag & drop
  2) Vercel   : folder upload karo, framework = "Other", build command khali
  3) GitHub Pages : repo mein index.html push karo -> Settings > Pages > main / root
  4) Cloudflare Pages : folder upload karo
  5) Normal hosting (cPanel/Hostinger) : index.html ko public_html mein upload karo

Dhyan rakhne wali baatein:
  - Site HTTPS pe host karo (sabhi upar wale services default HTTPS deti hain).
  - Fonts Google Fonts se load hote hain, isliye user ke paas internet chahiye.
  - Voice (bolne wali) feature Google Translate TTS fallback use karta hai; ye
    unofficial hai, kabhi block ho sakta hai. Tab text normal dikhega, site nahi tootegi.
  - Farmer ka data sirf us user ke browser (localStorage) mein save hota hai.
