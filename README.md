# veeva-QMS-Record-Attachments-Bulk-Downloads

### Need of this script, WHY?
During Migration, There may be requirement to trasfer the associated QMS record attachments. Once can configure the User Action to tag Formatted output report in the attchment section of any QMS record. Script will download Formatted Output Report and all attachments tagged with any QMS record in Bulk. 

### General tips for this script before execution
1. Pyhton scripting has been executed on the Jupiter notebook. One can get help of this script and use it in other coding tools as well.
2. Script also generate the log file to identify if for any attchment Ids - It failed to download the Content.
3. "Credentials.txt" file contains the Vault Username, Password,environment URL and the veeva API version. One can use the latest version of API by editing the "credentials.txt" file.
4. Script contains your session IDs for vault authentication(Basic Security policy). USE your test environment before the PROD executions.
5. For bulk downloading the Attachments - One will have Report configured in as QMS Record with Attachments (required column - Attchment Id, Record ID, Record Name). One will 6. download this report in CSV format and use it in script to download the attachments.
Script is designed in a way where it will download attachments for one QMS record type  at one time.
