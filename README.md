# veeva-QMS-Record-Attachments-Bulk-Downloads

### Need of this script, WHY?
During Migration, There may be the requirement to trasfer the associated QMS record attachments and formatted o/p reports. For fomatted o/p report, One can configure the User Action which will include Formatted output report as an attachment in the attchment section of any QMS record. Script will download Formatted Output Report and all other attachments tagged with any QMS record in Bulk. 

### General tips for this script before execution
1. Pyhton scripting has been executed on the Jupiter notebook. One can get help of this script and use it in other tools as well.
2. Script also generate the log file to identify if for any attchment Ids - It failed to download the Content.
3. "Credentials.txt" file contains the Vault Username, Password,environment URL and the veeva API version. One can use the latest version of API by editing the "credentials.txt" file.
4. Script contains your session IDs for vault authentication(Basic Security policy). USE your test environment before the PROD executions.
5. For bulk downloading the Attachments - QMS Record with Attachments report in csv format is required(required column - Attchment Id, Record ID, Record Name). One will download this report in CSV format and use it in script to download the attachments.
6. Script is designed in a way where it will read one attachment ID from csv report, download all the tagged attachments and repeat the process till the last attachment ID from the csv report. 
