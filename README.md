# RepliDocs App
(Full-Stack Development) My replica to Google Docs App using Flutter, also using Node.js, Express Sockets, MongoDB, Riverpod, and various techniques. The replica application contains methods of authenticating users with Google, keeping users logged in, creating RestAPI to create and display new documents, building a powerful routing system to share documents links, and establishing socket connection to allow users to collaborate.
## ***[Copyright and Commercial Use Disclaimer](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#please-carefully-read-licensemd-about-the-open-source-restrictions-and-the-personal-use-policy-of-this-project-under-gpl-30-license-any-commericial-uses-on-this-project-by-other-than-the-owner-krystalzhang612-or-the-authorized-users-and-organizations-including-unauthorized-modifications-forks-pull-requests-and-other-commercial-related-uses-will-be-subjected-to-copyright-violation-with-sebsequent-legal-concerns)***

⏬

### ***Please carefully read [LICENSE.md](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/LICENSE) about the Open Source restrictions and the personal use policy of this project under [GPL-3.0 license](https://www.gnu.org/licenses/gpl-3.0.en.html), any commericial uses on this project by other than the owner [@KrystalZhang612](https://github.com/KrystalZhang612) or the authorized users and organizations, will be subjected to copyright violation with sebsequent legal potential concerns.***
`NOTE:` Must run the project at where the `flutter` directory at. 
## RepliDocs App Overview:
![Screenshot](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/RepliDocs%20App%20Overview.PNG)<br/>
# Build
[Method to Run & Test the Project Locally](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#method-to-run--test-the-project-locally)<br/>
[Prerequisites & Setups](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#prerequisites--setups)<br/> 
[Debugging&Troubleshooting](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#debuggingtroubleshooting)<br/> 
[Synchronous Developing Notes](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#synchronous-developing-notes)<br/>
[Testing Result](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#testing-result)<br/> 
[Tags and Topics](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#tags-and-topics)<br/>
# Contribution
[Author](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md#author)
# Functionalities/Demo
- Contains a neat navbar.
- Allows users to sign in, sign out, authenticate with Google and staying logged in.
- Creating a New Document.
- Displaying all documents created by the user.
- Contains a well-designed Document Screen.
- Contains Collaborative Editing.
- Auto-Save functionality works.
- Sharing Link works.
# Compatibility
|   OS             | Supported          |
| -------          | ------------------ |
| macOS            | :white_check_mark: |
| Android          | :white_check_mark: |
| Linux            | ✅                 |
| web server       | ✅                 |
# Method to Run & Test the Project Locally
### Download the entire project to the local directory. 
### Open the project with Vscode. 
### Run `npm install` to initialize node.js
### Download needed dependencies, extension tools and MongoDB refer to [README](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md). 
### Use command  `ipconfig getifaddr en0` or  `ipconfig getifaddr en1` in the local device terminal to obtain your local private ip address. 
### Replace `<your ip address>` in [`repli_docs_app/lib/constants.dart`](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/lib/constants.dart) with your own ip address. 
### Open 2 different Vscode terminals. 
### In terminal 1: use `cd repli_docs_app` to locate the App root. 
### In terminal 2: use `cd server` to locate to `index.js`, `node.js` server.
In [Thunder Client extension](https://www.thunderclient.com/), send a new POST request at http://localhost:3001/api/signup with the JSON body filling out with: 
```bash
{
  "name": "YOUR OWN USERNAME FROM MONGODB", 
  "email": "YOUR OWN EMAIL ADDRESS FROM MONGODB", 
  "profilePic": "YOUR OWN PASSWORD FROM MONGODB"
}
```
### Run `npm run dev` in node terminal until it returns “connection successful”.
### Then run `flutter run -d chrome --web-port 3000`
### Have fun testing the replica of Google Docs Clone -> RepliDocs App! 

# 🛠️ Developing Languages, Tools, and Techniques Needed
[Flutter Dart Code v3.52.0 Vscode Extension](https://marketplace.visualstudio.com/items?itemName=Dart-Code.flutter)<br/>
[Flutter SDK](https://docs.flutter.dev/get-started/install/macos)<br/>
[Vscode 1.73](https://code.visualstudio.com/updates/v1_73)<br/> 
[Dart programming language](https://dart.dev)<br/> 
[dart google_sign_in dev dependency 5.4.2](https://pub.dev/packages/google_sign_in)<br/>
[Google Console Cloud API](https://console.cloud.google.com/projectselector2/apis/dashboard?pli=1&supportedpurview=project)<br/> 
[Xcode 14.1](https://developer.apple.com/documentation/xcode-release-notes/xcode-14_1-release-notes)<br/> 
[Flutter Riverpod Dependency](https://codewithandrea.com/articles/flutter-state-management-riverpod/)<br/>
[Node.JS v18.12.0](https://nodejs.org/en/)<br/>
[NPM JS](https://www.npmjs.com)<br/> 
[Socket Express](https://socket.io/get-started/chat/)<br/>
[JSON Web Token](https://www.npmjs.com/package/jsonwebtoken)<br/> 
[Mongoose](https://www.npmjs.com/package/mongoose)<br/> 
[MongoDB Cloud](https://www.mongodb.com)<br/> 
[Thunder Client Vscode extension v2.0.0](https://www.thunderclient.com/)<br/>
[JSON Web Tokens](https://jwt.io/)<br/>
[routemaster](https://pub.dev/packages/routemaster)<br/> 
[Flutter Riverpod Snippets](https://marketplace.visualstudio.com/items?itemName=robert-brunhage.flutter-riverpod-snippets)<br/> 
[AutoDraw](https://www.autodraw.com/)<br/> 
[Flutter Quill](https://pub.dev/packages/flutter_quill)<br/> 
[socket_io_client](https://pub.dev/packages/socket_io_client)<br/> 
[C++](https://cplusplus.com/)<br/>
[CMake](https://cmake.org/)<br/>
[JavaScript](https://javascript.com/)<br/>
[HTML5](https://en.wikipedia.org/wiki/HTML5)<br/>
[Swift5.7](https://docs.swift.org/swift-book/)<br/>
<div>
  <img src="https://github.com/devicons/devicon/blob/master/icons/dart/dart-original.svg" title="dart" alt ="dart" width="60" height="60"/>&nbsp; 
  <img src ="https://github.com/devicons/devicon/blob/master/icons/flutter/flutter-original.svg" title="futter" alt ="flutter" width="60" height="60"/>&nbsp;  
  <img src = "https://github.com/devicons/devicon/blob/master/icons/vscode/vscode-original.svg" title="vscode" alt ="vscode" width="60" height="60"/>&nbsp;  
  <img src ="https://github.com/devicons/devicon/blob/master/icons/googlecloud/googlecloud-original.svg" title="google-cloud-console-api" alt ="google-cloud-console-api" width="60" height="60"/>&nbsp;  
  <img src ="https://github.com/devicons/devicon/blob/master/icons/xcode/xcode-original.svg" title="xcode" alt ="xcode" width="60" height="60"/>&nbsp; 
  <img src ="https://github.com/devicons/devicon/blob/master/icons/nodejs/nodejs-original.svg" title="nodejs" alt ="nodejs" width="60" height="60"/>&nbsp; 
  <img src ="https://github.com/devicons/devicon/blob/master/icons/npm/npm-original-wordmark.svg" title="npm" alt ="npm" width="60" height="60"/>&nbsp; 
  <img src ="https://github.com/devicons/devicon/blob/master/icons/mongodb/mongodb-original.svg" title="mongodb" alt ="mongodb" width="60" height="60"/>&nbsp; 
  <img src ="https://github.com/devicons/devicon/blob/master/icons/cplusplus/cplusplus-original.svg" title="cpp" alt ="cpp" width="60" height="60"/>&nbsp;
  <img src ="https://github.com/devicons/devicon/blob/master/icons/cmake/cmake-original.svg"  title="cmake" alt ="cmake" width="60" height="60"/>&nbsp;
  <img src ="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" title="javascript" alt ="javascript" width="60" height="60"/>&nbsp;
  <img src ="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" title="html5" alt ="html5" width="60" height="60"/>&nbsp;
  <img src ="https://github.com/devicons/devicon/blob/master/icons/swift/swift-original.svg"  title="swift" alt ="swift" width="60" height="60"/>&nbsp;    
</div>

# Prerequisites & Setups
Install Flutter Dart Code extension in Vscode empty starting page.<br/>
Install Flutter SDK to the desired local directory. <br/> 
Configure and export Flutter to the local path in Console:
```bash
export PATH="$PATH:`pwd`/flutter/bin"
```
Use Command Palette in Vscode-> Flutter -> Create a new project -> Application.<br/>
To avoid macOS “zsh command not found” error:<br/> 
In Console, run `vim $HOME/.zshrc`<br/>
Press the "I" key to go into INSERT mode.<br/> 
Add the following line in the opened file:
```bash 
export PATH=$PATH:/Desktop/flutter/bin
```
Press "Esc" then write `:wq!` in terminal and press enter to exit vim.<br/> 
Restart the created Flutter project in Vscode.<br/> 
In Vscode Terminal, `navigate to the Flutter project first`:
```bash 
cd FLUTTER_PROJECT_NAME
```
Then run the Flutter project with:
```bash
flutter run
```
Choose Chrome Web/macOS Safari for testing.<br/> 
Done setting up when `Flutter Demo` web server successfully launched in browser.<br/>
[flutter project web server done setting up.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/flutter%20project%20web%20server%20done%20setting%20up.PNG)<br/>
# Synchronous Developing Notes
Pass Google logo for the signin page in [login_screen.dart](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/lib/screens/login_screen.dart):
```dart
import 'package:flutter/material.dart';
class LoginScreen extends StatelessWidget {
  const LoginScreen({Key? key}) : super(key: key);
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Center(
        child: ElevatedButton.icon(
          onPressed: () {},
          icon: Image.asset('assets/images/google-icon.png'),
          label: const Text(
            'Sign in with Google'
```
[google icon imported.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/google%20icon%20imported.PNG)<br/>
Resize it and we got:<br/>
[google icon resized to height 20.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/google%20icon%20resized%20to%20height%2020.PNG)<br/>
Create OAuth client ID with Google Console Cloud API.<br/>
`NOTE`: Actively use command `flutter clean` and `flutter run` to rebuild from root.<br/> 
Configure for Android and append [google_services.JSON](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/android/app/google_services.json)<br/>
Configure for iOS: Open it with Xcode-> input bundle ID-> download plist. <br/>
Configure web applications refer to the pub dev page.<br/> 
Set preferable localhost at port 3000.<br/> 
Now in Vscode run:
```bash
 flutter run -d chrome --web-port 3000
```
Now passed the web server at localhost:3000 successfully:<br/>
[web server passed to localhost 3000.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/web%20server%20passed%20to%20localhost%203000.PNG)<br/>
## ***Configure Google sign in using Node.js:***
Install Riverpod dependency:<br/>
add 
```yaml
add flutter_riverpod: ^2.0.0-dev.9
```
in [pubspec.yaml](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/pubspec.yaml)<br/> 
Run `dart pub get` in the Vscode terminal.<br/>
Import Riverpod in [auth_repository.dart](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/lib/repository/auth_repository.dart):
```dart
import 'package:flutter_riverpod/flutter_riverpod.dart';
```
Add Riverpod provider for login auth:
```dart
final authRepositoryProvider = Provider(
  (ref) => AuthRepository(
...
```
Run flutter web server again. The google account sign-in page popped:<br/> 
[google account sign-in page popped.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/google%20account%20sign-in%20page%20popped.PNG)<br/> 
Sign in to my google account:<br/> 
[signed in.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/signed%20in.PNG)<br/>
Use npm in Vscode to install Express socket, JSONWEBTOKEN and Mongoose:
```bash
 npm i express http socket.io@2.3.0 jsonwebtoken mongoose
```
Install Nodemon:
```bash
npm i nodemon --save-dev
```
Use `npm run de` to start the server at port 3001 based on [index.js](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/server/index.js):
```JavaScript
const express = require("express");
const mongoose = require("mongoose");
const PORT = process.env.PORT | 3001;
const app = express();
app.listen(PORT, "0.0.0.0", () => {
    console.log(`connected at port ${PORT}`);
});
```
server connected.<br/>
## ***Connect to MongoDB:***
```JavaScript
mongoose
    .connect(DB)
    .then(() => {
        console.log("Connection successful!");
    })
    .catch((err) => {
        console.log(err);
    })
//async -> await
// .then((data) => print(data))
app.listen(PORT, "0.0.0.0", () => {
    console.log(`connected at port ${PORT}`);
});
```
Set up MongoDB and run the server `npm run dev` again:<br/>
[mongodb connection successfully.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/mongodb%20connection%20successful.PNG)<br/>
Configure local private IP address to be redirect to signup page at port 3001: Use command in local terminal:
```bash
ipconfig getifaddr en0/1
```
To obtain the local private IP address, and in constants.dart: 
```dart
const host = ‘<ip address>:3001`
```
Then in auth_repository.dart, pass host:
```dash
 var res = await _client.post(Uri.parse('$host/api/signup'),
            body: userAcc.toJson(),
            headers: {
              'Content-Type': 'application/json; charset=UTF-8',
});
```
Now rerun both node and dart terminals on vscode:<br/>
[redirected to signup 3001 page.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/redirected%20to%20signup%203001%20page.PNG)<br/>
Use `flutter pub add shared_preferences` in dart terminal to install shared_pref lib.<br/>
Use `flutter pub add routemaster` to install routemaster.
## ***Create new documents:***
Set up id and routers when creating new document in [router.dart](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/lib/router.dart):
```dart
final loggedInRoute = RouteMap(routes: {
  '/': (route) => const MaterialPage(child: HomeScreen()),
  '/document/:id/:somethingelse': (route) => MaterialPage(
        child: DocumentScreen(
          id: route.pathParameters['id'] ?? '',
), ),
```
Parse Uri of my docs in [document_repository.dart](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/lib/repository/document_repository.dart):
```dart
Uri.parse('$host/docs/me'),
```
[new document id showed.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/new%20document%20id%20showed.PNG)<br/>
[list of untitled documents parsed.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/list%20of%20untitled%20documents%20parsed.PNG)<br/>
Design document sharing button in [document_screen.dart](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/repli_docs_app/lib/screens/document_screen.dart):
```dart
Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        backgroundColor: kWhiteColor,
        elevation: 0,
        actions: [
          ElevatedButton.icon(
            onPressed: () {},
            icon: const Icon(
Icons.lock,
size: 16,
```
[document sharing button.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/document%20sharing%20button.PNG)<br/>
Design document title in document_screen.dart:
```dart
title: Row(
          children: [
            Image.asset(
              'assets/images/google-docs-logo.png',
              height: 40,
            ),
            const SizedBox(width: 10),
            SizedBox(
              width: 180,
              child: TextField(
                controller: titleController,
                decoration: const InputDecoration(
                  border: InputBorder.none,
            contentPadding: EdgeInsets.only(left: 10),
```
[document title design.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/document%20title%20design.PNG)<br/>
Use `flutter pub add flutter_quill` to install flutter quill.
## ***Import Quill editor:***
```dart
import 'package:flutter_quill/flutter_quill.dart' as quill;
   body: Column(
          children: [
            quill.QuillToolbar.basic(controller: _controller),
            Expanded(
              child: quill.QuillEditor.basic(
                controller: _controller,
    readOnly: false, // true for view only mode
```
[quill editor banner showed.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/quill%20editor%20banner%20showed.PNG)<br/>
Make the text editor canvas align at center:
```dart
 body: Center(
        child: Column(
          children: [
            quill.QuillToolbar.basic(controller: _controller),
            Expanded(
              child: SizedBox(
                width: 750,
                child: Card(
                  color: kWhiteColor,
                  elevation: 5,
                  child: quill.QuillEditor.basic(
                    controller: _controller,
                    readOnly: false, // true for view only mode
```
[text editing canvas align at center.PNG](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/text%20editing%20canvas%20align%20at%20center.PNG)<br/> 
bold, italic, underline, different text colors and various text effects testing:<br/>
![Screenshot](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/various%20text%20effects%20testing.PNG)<br/>
Install socket_io_client with:
```bash
flutter pub add socket_io_client
```
generate public sharing link in document_screen.dart:
```dart
Clipboard.setData(ClipboardData(
text:
'http://localhost:3000/#/document/${widget.id}'))
              .then(
                 (value) {
         ScaffoldMessenger.of(context).showSnackBar(const SnackBar(
                        content: Text(
                          'Link copied!'
```
Now click on Share button, a public sharing link will be generated.

# Debugging&Troubleshooting
- Error: `Cannot run with sound null safety, because the following
dependencies don't support null safety: - package:http -
package:http_parser For solutions, see` https://dart.dev/go/unsound-null-safety
DEBUGGING: Update flutter http to the latest version.
- Git Flutter speed up: git push hangs after Total line. DEBUGGING: Increase buffer: run `git config --global http.postBuffer 157286400`.
- XHTTPEmpty Error: Failed to connect to Mongoose and API server to get response. DEBUGGING: Reconnect to Mongoose-> Node terminal-> `npm run dev` -> Locate errors and debug errors -> Thunder Client -> Send new Request http://localhost:3001/api/signup -> Node run again-> mongoose reactivated -> Dart terminal run.

# Testing Result

<p align = "center">
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/flutter%20project%20web%20server%20done%20setting%20up.PNG">&nbsp;
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/google%20icon%20imported.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/google%20icon%20resized%20to%20height%2020.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/web%20server%20passed%20to%20localhost%203000.PNG">&nbsp;
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/google%20account%20sign-in%20page%20popped.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/signed%20in.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/mongodb%20connection%20successful.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/redirected%20to%20signup%203001%20page.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/new%20document%20id%20showed.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/list%20of%20untitled%20documents%20parsed.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/document%20sharing%20button.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/document%20title%20design.PNG">&nbsp; 
  <img src = "https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/testing-result-repli_docs_app/quill%20editor%20banner%20showed.PNG">&nbsp; 
</p> 




# Tags and Topics
full-stack, flutter, dart, vscode, google-docs-clone, google-console-cloud-api, xcode, node-js, npm, socket-express, json-web-tokens, mongodb, thunder-client, routemaster, riverpod, flutter-quill, socket-io-client, javascript, cpp, cmake, html5, swift5.7. 
# Author
Krystal Zhang
https://github.com/KrystalZhang612<hr>
*This file was generated by [RepliDocsApp-readme](https://github.com/KrystalZhang612/KrystalZhang-Repli-Docs-App/blob/main/README.md), on November 11th, 2022*

