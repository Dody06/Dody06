### Importing from other apps

[Google Authenticator](https://github.com/jamie-mh/AuthenticatorPro/wiki/Importing-from-Google-Authenticator)

[Blizzard Authenticator](https://github.com/jamie-mh/AuthenticatorPro/wiki/Importing-from-Blizzard-Authenticator)

[Steam](https://github.com/jamie-mh/AuthenticatorPro/wiki/Importing-from-Steam)

### Authy

Authenticator Pro can generate the 7 digit codes used by Authy. Unfortunately, there is no way to export the secrets directly from the Authy app as it's locked down and proprietary.

*This guide may require some advanced technical knowledge*

The procedure is as follows:

- Use the ``authy-export`` tool found here : https://github.com/alexzorin/authy to generate an otpauth URI list file.
- Import the file in Authenticator Pro using the URI list import option.

Because of the way Authy generates codes, you are not able to delete your Authy account as this invalidates the secrets.

