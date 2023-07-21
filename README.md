# ILLiad Alma NCIP Lending V1.2

Hello and Welcome!

This is the official GitHub repository containing the latest updates for the ILLiad Alma NCIP Lending System Addon.   The latest version of this Addon submitted to Atlas Systems can be found at the [ILLiad Addons Directory](https://atlas-sys.atlassian.net/wiki/spaces/ILLiadAddons/pages/3149522/ILLiad+ALMA+NCIP+Borrowing+Client+System+Addon).  

This is a System Addon for [ILLiad](https://www.atlas-sys.com/illiad) allowing for automated checking out of Lending items in Alma from ILLiad via NCIP, using a item barcode stored from data within a selectable ILLiad transaction field.

This System Addon needs to be installed in the same directory as your regular Addons in its own folder.  If you make changes to your Addon configurations through the [config.xml](https://github.com/Hypolymer/ILLiad_Alma_NCIP_Lending/blob/main/config.xml) file while your ILLiad Client is open, you will need to close and reopen your ILLiad Client for the configuration changes to take effect.  You may also make changes to your configuration values through the ILLiad Client, under System > Manage Addons.

If you run into problems and want to see the error log, please check these instructions:  https://github.com/Hypolymer/AddonsLibrary/wiki/Enabling-ILLiad-Client-and-Server-Logs

This System Addon is typically used in conjunction with the [ILLiad Alma NCIP Borrowing Addon](https://github.com/Hypolymer/ILLiad_Alma_NCIP_Borrowing/)  and the [ILLiad Alma NCIP Borrowing Renewals V2 Addon](https://github.com/Hypolymer/ILLiad_Alma_NCIP_Borrowing_Renewals_V2).

Description of Addon Configuration Settings ([config.xml](https://github.com/Hypolymer/ILLiad_Alma_NCIP_Lending/blob/main/config.xml))
| Configuration Value        | Description |
|:------------- | :-----|
|NCIP_Responder_URL|The URL used to connect to your Alma NCIP responder. Replace "xxx" with your institution's three letter Alma code. If SUNY, replace "xxx" with "suny-zzz", and replace zzz with your institution's three letter Alma code.|
|ILLiad_field_to_get_barcode|This field will be used as the item barcode in Alma (the ItemInfo3 field is the default setting).|
|acceptItem_from_uniqueAgency_value|Replace "XXX" with your institution's three letter Alma code.  If SUNY, replace "XXX" with "SUNY_ZZZ", and replace ZZZ with your institution's three letter Alma code.|
|ApplicationProfileType|Input the Resource Sharing Partner code used in Alma.  Possible values might be "ILL" or "ILLiad".|
|LendingCheckOutItemFailQueue|This designates the name of the queue a Lending Transaction will be moved to if the CheckOutItem function fails. Queue names that do not currently exist will be created automatically.|
|LendingCheckInItemFailQueue|This designates the name of the queue a Lending Transaction will be moved to if the CheckInItem function fails. Queue names that do not currently exist will be created automatically.|
