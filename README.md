# Standard Hybrid Mobile App Structure Mokup
Currently in Work-In-Progress Status
## Roadmap
- Completing the guide (maybe translate?)
- Write the example project
- Update the guide to MultiApp Structure
- Write the MultiApp Example
## General Purpose structure
 - AppModule (that must implements Injection Tokens to spread the environment)
	- CoreModule: App Level Single Imports
		- Language set up
		- Error Handling
		- Environment Modelling
		- Storage
		- Analytics
		- App Status (isLogged, isConnected, etc)
	- AuthenticationModule: Authentication Singleton Imports
		- Authentication Service
		- Navigation Guards
		- Token Validation
	- CommonsModule: Business Level Signleton Imports
		- Push Notifications Subscription
		- Cordova Plugin abstactions (Geo, Camera, InAppBrowser, etc.
	- SharedModule: Business Level Non-Singleton Imports
		- Directives
		- Common Models
	- CustomModule:
	- PageModule:

=================
# Idea Mockups
## DO NOT IMPLEMENT
### Components Workflow
Finite statuses; Active, Inactive, Busy, onError [...] driven by directive.
StatusChange Callback.
Contemplate CDK Overlay Directive
