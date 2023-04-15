# remove android bloat

0. enable developer options
1. enable usb debugging
2. `adb devices` (you need android sdk platform tools)
3. `adb shell cmd package uninstall -k --user 0 com.package.name`

(the `--user 0` flag allows us to uninstall pre-installed apps, most of the time)

here's a list i used on a xiaomi phone a few years back:
```sh
adb shell cmd package uninstall -k --user 0 com.android.chrome
adb shell cmd package uninstall -k --user 0 com.android.calendar
adb shell cmd package uninstall -k --user 0 com.miui.calculator
adb shell cmd package uninstall -k --user 0 com.android.browser
adb shell cmd package uninstall -k --user 0 com.miui.analytics
adb shell cmd package uninstall -k --user 0 com.google.android.youtube
adb shell cmd package uninstall -k --user 0 com.google.android.apps.photos
adb shell cmd package uninstall -k --user 0 com.miui.notes
adb shell cmd package uninstall -k --user 0 com.miui.player
adb shell cmd package uninstall -k --user 0 com.duokan.phone.remotecontroller
adb shell cmd package uninstall -k --user 0 com.google.ar.lens
adb shell cmd package uninstall -k --user 0 com.google.android.tts
adb shell cmd package uninstall -k --user 0 com.google.android.music
adb shell cmd package uninstall -k --user 0 com.google.android.videos
adb shell cmd package uninstall -k --user 0 com.google.android.googlequicksearchbox
adb shell cmd package uninstall -k --user 0 com.google.android.gm
adb shell cmd package uninstall -k --user 0 com.google.android.inputmethod.latin
adb shell cmd package uninstall -k --user 0 com.xiaomi.glgm
adb shell cmd package uninstall -k --user 0 com.facebook.services
adb shell cmd package uninstall -k --user 0 com.facebook.appmanager
adb shell cmd package uninstall -k --user 0 com.facebook.system
adb shell cmd package uninstall -k --user 0 com.google.android.apps.tachyon
adb shell cmd package uninstall -k --user 0 com.google.android.apps.docs
adb shell cmd package uninstall -k --user 0 com.google.ar.core
adb shell cmd package uninstall -k --user 0 com.xiaomi.midrop
adb shell cmd package uninstall -k --user 0 com.mipay.wallet.in
adb shell cmd package uninstall -k --user 0 com.mi.globalTrendNews
adb shell cmd package uninstall -k --user 0 com.android.calendar
adb shell cmd package uninstall -k --user 0 com.mipay.wallet.id
adb shell cmd package uninstall -k --user 0 com.miui.bugreport
adb shell cmd package uninstall -k --user 0 com.xiaomi.payment
adb shell cmd package uninstall -k --user 0 com.miui.cloudbackup
adb shell cmd package uninstall -k --user 0 com.miui.cloudservice
adb shell cmd package uninstall -k --user 0 com.miui.micloudsync
adb shell cmd package uninstall -k --user 0 com.miui.videoplayer
```
