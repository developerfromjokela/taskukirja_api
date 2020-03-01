# Taskukirja API Reverse-Engineered
Reverse-Engineered Taskukirja API Documentation

In this repository, I will make an documentation how to use Taskukirja API in your projects.

#### What is Taskukirja? Never heard about
Taskukirja is a Android application for Finnish libraries for easy access to its services on mobile.

#### One extra info about Taskukirja, pay attention!
There are several "Clone apps", in some cases identical apps of Taskukirja app. 
They have different API Server.

Taskukirja app: https://taskukirja.enisoft.fi/prd
KirjastoON app: https://aurora-kerava.enisoft.fi/prd

## Documentation Root
- Login Request (`login_request.md`)

## How can I reverse-engineer more stuff?

Simple, the app is written in Xamarin, and you can extract DLLs from APK and read the whole source code.

You can use tools such as ILSpy or dotPeek to read the source code.
Extract the APK using some unzip program. DLLs are in folder "assemblies"
The API class contains in package `PocketLibraryClientCommon.WebClients.RestClient`

## I don't hold any responsibility on what are you doing with this discovery.
If you do something bad and harmful using my documentation, you're responsible for it, I don't hold any liability.

Note: this API's maintainer can change something and my documentation will be outdated,
