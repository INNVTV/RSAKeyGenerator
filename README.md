# RSAKeyGenerator
Generates RSA keys using both XML String and PEM formats using C#/.Net Core 

### RSACryptoServiceProviderExtensions
.Net Core does not properly implement .ToXmlString() on RSACryptoServiceProvider so we implement the custom extension methods found in the RSACryptoServiceProviderExtensions.cs file in the project root. 

### XMLString Format(s)
The XML String format is the default for encryption and signging JWT tokens in the .Net framework. You use the FromXmlRsaString_PublicOnly and FromXmlRsaString_PublicOnly and ToXmlRsaString_Full extension methods to read in XML strings and the FromXmlRsaString_Full and FromXmlRsaString_PublicOnly extension methods to import/export this format.

### PEM Format(s)
Privacy-Enhanced Mail (PEM) is a de facto file format for storing and sending cryptographic keys, certificates, and other data, based on a set of 1993 IETF standards.
