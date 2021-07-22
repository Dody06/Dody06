Welcome to the Authenticator Pro wiki!

## Quick Links

[Contribution Guide](https://github.com/jamie-mh/AuthenticatorPro/blob/master/CONTRIBUTING.md)

[Backup File Format](https://github.com/jamie-mh/AuthenticatorPro/blob/master/doc/BACKUP_FORMAT.md)

### Importing from other apps

[Google Authenticator](https://github.com/jamie-mh/AuthenticatorPro/wiki/Importing-from-Google-Authenticator)

[Blizzard Authenticator](https://github.com/jamie-mh/AuthenticatorPro/wiki/Importing-from-Blizzard-Authenticator)

[Steam](https://github.com/jamie-mh/AuthenticatorPro/wiki/Importing-from-Steam)

[Authy](https://github.com/jamie-mh/AuthenticatorPro/wiki/Importing-from-Authy)

## Frequently Asked Questions

**Is Authenticator Pro available / coming to iOS?**

No and probably not. Publishing an app on the App Store requires that you pay an annual $99 fee. Furthermore, you must own Apple hardware to develop an app in the first place.

**Will you implement [feature]?**

Maybe. Create an issue and fill out the "Feature request" template.

**Can you add an icon?**

Yes. Create a request in a GitHub issue or [do it yourself](https://github.com/jamie-mh/AuthenticatorPro/blob/master/CONTRIBUTING.md#icons) if you'd like.

**Can you add sync to Google Drive, OneDrive, etc...**

No. Syncing to cloud services would require the internet permission and heavy intrusive SDKs to support them. Also, they have a habit of changing the APIs often, which just requires more work.

**I've entered the code and it's not working, what should I do?**

Make sure that the time on your device is correct. Sync with a mobile network if possible for better accuracy.

**Why doesn't Google Drive, OneDrive, Dropbox, etc... appear in the auto-backup storage location list?**

The dialog you see when you select a storage location is not part of Authenticator Pro but rather part of Android. The Storage Access Framework as it is named, receives varying levels of support from cloud providers. If the provider of your choice does not appear, then this is a limitation of their app.

Fully supporting it is possible (Nextcloud for instance), but this may not be a high priority for the developers. A way around this would be to backup to a folder on your device and then use a 3rd party to sync the contents of that to cloud storage. First party support for cloud services will not be implemented, see above.

**Can you add import for [alternative authenticator app]?**

It depends if the app supports exporting your data to a file. For instance, Microsoft Authenticator doesn't allow you to export your secrets, but rather only lets you sync with your Microsoft account. Your data is locked in and thus it's impossible to transfer to Authenticator Pro without disabling and re-enabling 2FA on all of your accounts.

**Does Authenticator Pro support [service]?**

Probably. Authenticator Pro supports TOTP, HOTP, mOTP and Steam which covers most of the services.

**How do I download the Wear OS companion app?**

Open Google Play on your watch and click Apps on Your Phone. You should see Authenticator Pro in the list and you can download it.

**I cannot access my accounts because I cleared the data on my phone without creating a backup. Can you help me?**

No. Use a recovery code to gain access. If you don't have one, you must contact the support of the service you are using.

**I cannot remember the password for my backup. Can you help me?**

See above

**I cannot remember the password for the app. Can you help me?**

See above

**I lost my phone, can you disable two factor authentication on my account(s)?**

No, Authenticator Pro generates codes offline, I have no access to your accounts. Contact the support of the service you are using.