# Security

A development machine should be secured against threads as well as any other machine (or even _especially_ a development machine). Therefore we will setup

* a firewall
* disk encryption

## Firewall

This one is a bit controversial. If you do not install software which allows network access of any kind, skip it. If you run potentially vulnerable software you don't want to be accessed from other machines, consider turning the built-in firewall on. This particularly applies if you develop network software.

To turn the built-in firewall on:

1. Choose Apple menu () > System Preferences, then click Security & Privacy.
2. Click the Firewall tab.
3. Click the Lock button, then enter an administrator name and password.
4. Click Turn On Firewall.
5. Click Firewall Options.
6. Uncheck 'Automatically allow signed software to receive incoming connections'.

The last step disables automatic access for software from the App Store. From now on you can either add (dis)allowed programs to the list within the Firewall Options or just click on Allow/Deny, if you get a popup asking you if a specific software may be accessed.

## Disk Encryption

Another controversial point. If you have a desktop machine in a secured building, you probably do not need disk encryption. If you travel a lot and take your notebook with you (including all your source codes), you might consider travelling with disk encryption enabled.

The following steps were taken from the [official apple support page](https://support.apple.com/en-us/HT204837) on this:

1. Choose Apple menu () > System Preferences, then click Security & Privacy.
2. Click the FileVault tab.
3. Click the Lock button, then enter an administrator name and password.
4. Click Turn On FileVault.
5. Follow the instructions. In my opinion you should create a local and offline possibility to disable encryption, when you are asked how to regain access in case of anything.

## Use a hardware key as a smart card

{% embed url="https://support.yubico.com/hc/en-us/articles/360016649059-Using-Your-YubiKey-as-a-Smart-Card-in-macOS" %}

## Add hardware key to iCloud account

{% embed url="https://www.yubico.com/blog/how-to-add-yubikeys-to-apple-id-a-step-by-step-guide/?gclid=EAIaIQobChMIn6OCxcjh_gIVMg99Ch3TqwIvEAAYASAAEgIc8_D_BwE" %}

Add hardware key to Google account

{% embed url="https://www.yubico.com/works-with-yubikey/catalog/google-accounts/" %}
