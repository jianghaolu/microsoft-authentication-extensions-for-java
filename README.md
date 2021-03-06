# Microsoft Authentication Library (MSAL) Extensions for Java

The extensions library for MSAL Java supports persistence of the cache to disk in encrypted form where the platform supports this. This is available for Mac, Windows and Linux. On Linux we depend on Libsecret and any place where libsecret is not available encryption is not supported. On Mac and Windows encryption support is built into the OS.

# Maven
You can find the latest pacakge in the [Maven repository](https://mvnrepository.com/artifact/com.microsoft.azure/msal4j-persistence-extension).

# PersistenceTokenCacheAccessAspect

Implementation of ITokenCacheAccessAspect interface defined in [Java MSAL SDK](https://github.com/AzureAD/microsoft-authentication-library-for-java)
for persistence of token cache in platform specific secret storage:
* Win - file encrypted with DPAPI
* Mac - key chain
* Linux - key ring

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
