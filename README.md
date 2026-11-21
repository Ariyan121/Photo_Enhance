# ফটো এনহান্স – Android প্রজেক্ট

ঝাপসা বা ছোট ছবিকে AI (ESRGAN Slim, UpscalerJS) দিয়ে ২×, ৩× বা ৪× বড় ও পরিষ্কার করার অ্যাপ। সবকিছু ফোনেই চলে, ছবি কোথাও আপলোড হয় না। মডেল ও TensorFlow.js অ্যাপের ভেতরেই আছে, তাই ইন্টারনেট ছাড়াই চলে।

## ক্লাউডে APK বানানো (GitHub Actions)

1. github.com-এ নতুন রিপোজিটরি বানান (যেমন `Photo_Enhance`)।
2. এই ফোল্ডারের ভেতরের সব ফাইল আপলোড করুন। `.github` ফোল্ডার বাদ পড়লে `.github/workflows/build-apk.yml` নামে ফাইল নিজে বানিয়ে ভেতরের লেখা পেস্ট করুন।
3. Actions ট্যাবে "Build Android APK" চলবে। সবুজ টিক এলে রানের নিচের Artifacts থেকে `photo-enhance-debug-apk` নামান, আনজিপ করলে `app-debug.apk` পাবেন।

## Play Store-এর আগে
- `capacitor.config.json`-এ `appId` বদলে অনন্য আইডি দিন, নিজস্ব আইকন যোগ করুন, সই করা AAB বানান।

## লাইসেন্স
UpscalerJS ও ESRGAN Slim মডেল: MIT। TensorFlow.js: Apache-2.0।
