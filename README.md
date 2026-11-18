# Fano Heren — Sky Defender

English HTML5 arcade shooter. Upload all files to the ROOT of a GitHub repository and enable GitHub Pages (Deploy from branch / main / root). Open the GitHub Pages HTTPS URL in PWABuilder to package for Windows. Test the built MSIX on a clean Windows machine before submitting to Microsoft Partner Center.

Controls: Left/Right or A/D, Space to fire, P to pause; touchscreen drag and hold to fire. Scores, best score and earned Gold are stored locally. Five shop entries: fano_gold_1 ($0.99, 100 Gold), fano_gold_2 ($4.99, 550 Gold), fano_gold_3 ($9.99, 1200 Gold), fano_gold_4 ($14.99, 1900 Gold), fano_gold_5 ($19.99, 2700 Gold).

IMPORTANT: The shop does NOT take payments. `window.FanoMicrosoftStore.purchase(productId)` is a documented hook for a FUTURE trusted Windows Store billing bridge, not an implemented payment SDK. In ordinary browser/PWA packaging the buttons explain that purchases are unavailable. Do not submit a paid IAP experience until a proper Microsoft Store SDK/GDK integration verifies completed transactions, grants the advertised Gold exactly once, handles retries and refunds, and passes certification. JavaScript alone cannot safely validate payments. Do not claim IAP is enabled in store listing until this is done.

The game works offline after initial installation. No external JS or fonts. Verify Play and Shop before publishing.
