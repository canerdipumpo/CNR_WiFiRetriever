WiFi Retriever Library | Made in KOSOVO with ❤️ by CNR Production®

Author: Caner di Pumpo
Version: v1.0
Update: v1.1
Date: 15.02.2020
Coded in: C# Language

Made by 15 year old Kosovar producer & programmer

? What is WiFi Retriever ?
WiFi Retriever helping to get list of saved SSIDs and Password. Its FREE and so easy!

Code Examples Here:

C# Example Code

using CNR_WiFiRetriever
public void RetrieveWiFi()
{
    var RetrieveWifi = CNR_RetrieveWiFi.RetrieveWiFi(); // Retrieve Wifi
    var SSIDsAndPaswords = new StringBuilder(); // Out of SSIDs and Passwrod
    var OnlySSIDs // Out of only SSIDs
    var OnlyPasswords // Out only Passwords
    foreach (var NetworkConnections in RetrieveWifi) // Start to Retrieve Wifi
    {
        SSIDsAndPaswords.AppendFormat("SSID: {0}", NetworkConnections.CNR_GetSSIDs).AppendLine().AppendFormat("Password: {0}", NetworkConnections.CNR_GetPasswords).AppendLine().AppendLine();
        OnlySSIDs.AppendFormat("SSID: {0}", NetworkConnections.CNR_GetSSIDs).AppendLine();
        OnlyPasswords.AppendFormat("Password: {0}", NetworkConnections.CNR_GetPasswords).AppendLine();
    }
}


VB.NET Example Code

Imports CNR_WiFiRetriever
  Public Sub RetrieveWiFi()
        Dim RetrieveWifi = CNR_RetrieveWiFi.RetrieveWiFi() ' Retrieve Wifi
        Dim SSIDsAndPaswords = New System.Text.StringBuilder() ' Out of SSIDs and Passwrod
        Dim OnlySSIDs ' Out of only SSIDs
        Dim OnlyPasswords ' Out only Passwords
        For Each NetworkConnections In RetrieveWifi ' Start to Retrieve Wifi
            SSIDsAndPaswords.AppendFormat("SSID: {0}", NetworkConnections.CNR_GetSSIDs).AppendLine().AppendFormat("Password: {0}", NetworkConnections.CNR_GetPasswords).AppendLine().AppendLine()
            OnlySSIDs.AppendFormat("SSID: {0}", NetworkConnections.CNR_GetSSIDs).AppendLine()
            OnlyPasswords.AppendFormat("Password: {0}", NetworkConnections.CNR_GetPasswords).AppendLine()
        Next
    End Sub
