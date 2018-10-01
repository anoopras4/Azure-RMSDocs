---
title: class mip FileEngine Settings 
description: Reference for class mip FileEngine Settings 
author: BryanLa
ms.service: information-protection
ms.topic: reference
ms.date: 09/27/2018
ms.author: bryanla
---
# class mip::FileEngine::Settings 
  
## Summary
 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
 public Settings(const std::string& engineId, const std::string& clientData, const std::string& locale)  |  [FileEngine::Settings](class_mip_fileengine_settings.md) constructor for loading an existing engine.
 public Settings(const Identity& identity, const std::string& clientData, const std::string& locale)  |  [FileProfile::Settings](class_mip_fileprofile_settings.md) constructor for creating a new engine.
 public const std::string& GetEngineId() const  |  Returns the engine ID.
 public const Identity& GetIdentity() const  |  Returns the engine Identity.
 public void SetIdentity(const Identity& identity)  |  Sets the engine identity.
 public const std::string& GetClientData() const  |  Returns the engine client data.
 public const std::string& GetLocale() const  |  Return the engine locale.
public void SetCustomSettings(const std::vector<std::pair<std::string, std::string>>& value)  |  Sets a list of name/value pairs used for testing and experimentation.
public const std::vector<std::pair<std::string, std::string>>& GetCustomSettings() const  |  Gets a list of name/value pairs used for testing and experimentation.
 public void SetSessionId(const std::string& sessionId)  |  Sets the engine session ID.
 public const std::string& GetSessionId() const  |  Return the engine session ID.
 public void SetProtectionCloudEndpointBaseUrl(const std::string& protectionCloudEndpointBaseUrl)  |  Sets the protection cloud endpoint base url, used to specify cloud boundary.
 public const std::string& GetProtectionCloudEndpointBaseUrl() const  |  Gets the cloudEndpointBaseUrl.
 public void SetProtectionOnlyEngine(const bool protectionOnly)  |  Sets protection only engine indicator - no policy/label.
 public const bool IsProtectionOnlyEngine() const  |  Return protection only engine indicator - no policy/label.
  
## Members
  
### Settings
[FileEngine::Settings](class_mip_fileengine_settings.md) constructor for loading an existing engine.

Parameters:  
* **engineId**: Set it to the unique engine ID generated by AddEngineAsync. 


* **clientData**: customizable client data that can be stored with the engine when unloaded, can be retrieved from a loaded engine. 


* **locale**: engine localizable output will be provided in this locale.


  
### Settings
[FileProfile::Settings](class_mip_fileprofile_settings.md) constructor for creating a new engine.

Parameters:  
* **identity**: Identity info of the user associated with the new engine. 


* **clientData**: customizable client data that can be stored with the engine when unloaded, can be retrieved from a loaded engine. 


* **locale**: engine localizable output will be provided in this locale.


  
### GetEngineId
Returns the engine ID.
  
### GetIdentity
Returns the engine Identity.
  
### SetIdentity
Sets the engine identity.
  
### GetClientData
Returns the engine client data.
  
### GetLocale
Return the engine locale.
  
### SetCustomSettings
Sets a list of name/value pairs used for testing and experimentation.
  
### GetCustomSettings
Gets a list of name/value pairs used for testing and experimentation.
  
### SetSessionId
Sets the engine session ID.
  
### GetSessionId
Return the engine session ID.
  
### SetProtectionCloudEndpointBaseUrl
Sets the protection cloud endpoint base url, used to specify cloud boundary.

Parameters:  
* **protectionCloudEndpointBaseUrl**: Base url associated with protection endpoints


  
### GetProtectionCloudEndpointBaseUrl
Gets the cloudEndpointBaseUrl.

  
**Returns**: Base url associated with protection endpoints
  
### SetProtectionOnlyEngine
Sets protection only engine indicator - no policy/label.
  
### IsProtectionOnlyEngine
Return protection only engine indicator - no policy/label.