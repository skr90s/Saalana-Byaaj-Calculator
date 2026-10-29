सालाना ब्याज कैलकुलेटर — Android प्रोजेक्ट

यह Android WebView ऐप का source project है। ऐप का calculator HTML asset के रूप में bundled है, इसलिए कैलकुलेशन ऑफलाइन चल सकता है।

महत्वपूर्ण:
- यह ZIP source project है, तैयार APK नहीं।
- इस वातावरण में Android SDK/Gradle build tools उपलब्ध नहीं हैं, इसलिए APK यहाँ compile नहीं किया गया।
- `.github/workflows/build-apk.yml` में GitHub Actions build workflow शामिल है।

मोबाइल से APK बनाने का एक तरीका:
1. GitHub पर नया repository बनाएँ।
2. इस ZIP को extract करके सभी files repository में upload करें (folder structure जस का तस रखें)।
3. Repository में Actions tab खोलें और “Build Android APK” workflow चलाएँ।
4. सफल build के बाद workflow run में “saalana-byaaj-debug-apk” artifact डाउनलोड करें।
5. ZIP artifact extract करके `app-debug.apk` डाउनलोड/इंस्टॉल करें। Android में “Install unknown apps” की अनुमति माँगी जा सकती है।

ध्यान दें:
- APK को install करने से पहले अपनी गणनाओं को जाँचें।
- PDF के लिए ऐप का print action Android print dialog खोलेगा; वहाँ Save as PDF चुनें।
