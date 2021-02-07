Authenticator Pro supports 8 digit codes and as such Blizzard Authenticator accounts are supported. However, Blizzard uses a proprietary algorithm for their account setup, so the accounts must be converted to standard TOTP.

## Method 1

*This guide expects that you are familiar with the Python pip package system*

The procedure is as follows:

- Install the required packages using pip: ``python-bna`` and ``python-qrcode`` by running ``pip3 install bna qrcode``.
- Follow the guide for the ``python-bna`` CLI to setup a new authenticator and generate a QR code: [https://github.com/jleclanche/python-bna/blob/master/README.md](https://github.com/jleclanche/python-bna/blob/master/README.md)

## Method 2 (Windows only)

1. Download the latest WinAuth version ("WinAuth-3.5.1.zip") from https://github.com/winauth/winauth/releases and extract its contents.

2. Double-click on the "WinAuth.exe" file to run it.

3. Click on "Add" ---> "Battle.Net" ---> "Create Authenticator". This will generate a serial number and an authenticator (a.k.a. Login) code. You'll need those for step # 6. Check the "Allow copy?" check box so you'll be able to copy those 2 codes to the clipboard.

4. Go to www.blizzard.com and log in to your account.

5. Go to "Account Settings" ---> "Security" and then click on "SET UP AN AUTHENTICATOR" ---> "Set up a mobile authenticator".

6. Enter the verification code sent to your Email/SMS to get through the security check.

7. Enter the serial number and authenticator code from step # 2 into the "ENTER AUTHENTICATOR INFORMATION" window and then click on "Add Authenticator" ---> "Back to security".

8. In the "WinAuth" window, click on "OK" ---> "Cancel" ---> "Cogwheel" ---> "Export..." ---> "Browse..." (DO NOT CHECK ANY OF THE 2 "Protect" CHECK BOXES!) ---> "Save" ---> "OK".

9. Open the "winauth-current year-current month-current day.txt" file you just created and copy its content (a single line of text) to the clipboard.

10. Go to https://www.qr-code-generator.com/ (or equivalent) and paste the line of text you just copied in step # 9 where it says "Enter your website, text or drop a file here". A QR code will be generated automatically.

11. Scan the QR code with the "Authenticator Pro" app and you're good to go!

12. Optional: In Authenticator Pro, change the issuer name to "Blizzard", the username to your username, and assign the "blizzard" icon manually.

13. Optional: Delete `winauth.xml` from `%appdata%\WinAuth` if you don't plan on keeping WinAuth on your computer.

### Sources

- https://www.reddit.com/r/Blizzard/comments/6pixcg/how_to_use_a_third_party_otp_app_for_2_step/
- https://github.com/winauth/winauth
