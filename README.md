



[![Docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://doc.servertribe.com)
[![Discord](https://img.shields.io/discord/844971127703994369)](http://discord.servertribe.com)
[![Docs](https://img.shields.io/badge/videos-watch-brightgreen.svg)](https://www.youtube.com/@servertribe)
[![Generic badge](https://img.shields.io/badge/download-latest-brightgreen.svg)](https://www.servertribe.com/community-edition/)

# Peek Build Field App






# Attune

[Attune](https://www.servertribe.com/)
automates and orchestrates processes to streamline deployments, scaling,
migrations, and management of your systems. The Attune platform is building a
community of sharable automated and orchestrated processes.

You can leverage the publicly available orchestrated blueprints to increase
your productivity, and accelerate the delivery of your projects. You can
open-source your own work and improve existing community orchestrated projects.

## Get Started with Attune, Download NOW!

The **Attune Community Edition** can be
[downloaded](https://www.servertribe.com/comunity-edition/)
for free from our
[ServerTribe website](https://www.servertribe.com/comunity-edition/).
You can learn more about Attune through
[ServerTribe's YouTube Channel](https://www.youtube.com/@servertribe).







# Clone this Project

To clone this project into your own instance of Attune, follow the
[Clone a GIT Project How To Instructions](https://servertribe-attune.readthedocs.io/en/latest/howto/design_workspace/clone_project.html).




## Blueprints

This Project contains the following Blueprints.



### Build Peek IOS Field App





## Parameters


| Name | Type | Script Reference | Comment |
| ---- | ---- | ---------------- | ------- |
| App Build Directory | Text | `appbuilddirectory` | The local macOS directory where the app will be built. |
| App Build Version | Text | `appbuildversion` | Example 12345678 |
| App Display Name | Text | `appdisplayname` |  |
| App Dot Version | Text | `appdotversion` | Example 1.2.3.4 |
| App Environment | Text | `appenvironment` | DEV, TEST, UAT, PROD |
| App Export Directory | Text | `appexportdirectory` | The directory where apps will be placed. /Users/peek/Downloads |
| App Icon File Name | Text | `appiconfilename` | The app icon to use. |
| App ID | Text | `appid` | The AppId to build Peek with, EG, com.synerty.peek |
| App Peek Hardcoded Host | Text | `apppeekhardcodedhost` |  |
| App Peek Hardcoded Host Port | Text | `apppeekhardcodedhostport` | The port for the app to connect to, for example 443 |
| App Peek Hardcoded Host Use SSL | Text | `apppeekhardcodedhostusessl` | true or false |
| App Primary Colour | Text | `appprimarycolour` | Leave unset for production. For DEV, TEST, etc, set this to the background colour you'd like the app to use, EG #ff9900 |
| Build for Production | Text | `buildforproduction` | Values: true or false |
| macOS Host | Linux/Unix Node | `macoshost` | The macOS host to build the app on. |
| macOS User | Linux/Unix Credential | `macosuser` | The unix user to login to the macOS host with |
| Peek Field App Source Linux User | Linux/Unix Credential | `peekfieldappsourcelinuxuser` |  |
| Peek Field App Source Node | Linux/Unix Node | `peekfieldappsourcenode` | The Peek server running the peek field service that we can pull the peek_field_app from. |
| Peek Field Service Host / IP | Text | `peekfieldservicehostip` | The hostname or IP address used to for the Peek Field App talk to the Peek Field Service |
| Peek Field Service Port | Text | `peekfieldserviceport` | The TCP Port used to for the Peek Field App talk to the Peek Field Service |
| Peek Field Service - Use SSL | Text | `peekfieldserviceusessl` | true or false - Should the Peek Field App expect to use SSL to talk to the Peek Field Service |
| XCode Auto Code Sign Style | Text | `xcodeautocodesignstyle` | Values: true or falce |
| XCode Provisioning Profile Name | Text | `xcodeprovisioningprofilename` |  |
| XCode Provisioning Profile UUID | Text | `xcodeprovisioningprofileuuid` |  |
| XCode Team | Text | `xcodeteam` |  |




## Files

| Name | Type | Comment |
| ---- | ---- | ------- |
| peek_field_app | Large Archives | SSH to the peek server, and run the following<br><br>```````[ "${USER}" == 'peek' ] || echo "You are NOT the peek user" >&2<br>cd<br><br>tar cvjf $(date "+%y%m%d_%H%M")_peek_field_app.tar.bz2 \<br>    --exclude node_modules \<br>    -C synerty-peek*/lib/python*/site-packages \<br>    peek_field_app<br><br> |
| Peek Icons | Version Controlled Files |  |






# Contribute to this Project

**The collective power of a community of talented individuals working in
concert delivers not only more ideas, but quicker development and
troubleshooting when issues arise.**

If you’d like to contribute and help improve these projects, please fork our
repository, commit your changes in Attune, push you changes, and create a
pull request.

<img src="https://www.servertribe.com/wp-content/uploads/2023/02/Attune-pull-request-01.png" alt="pull request"/>

---

Please feel free to raise any issues or questions you have.

<img src="https://www.servertribe.com/wp-content/uploads/2023/02/Attune-get-help-02.png" alt="create an issue"/>


---

**Thank you**
