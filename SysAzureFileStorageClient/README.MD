Azure File storage client.

Usage:

        SysAzureFileStorageClient_IM fileClient = SysAzureFileStorageClient_IM::newFromAzureStorageAccountNameShare('mystorageaccountname', 'mysharename');

        System.IO.MemoryStream memoryStream = fileClient.readToStream('MyFile.txt');

        var txt = new System.IO.StreamReader(memoryStream).ReadToEnd();

        info (txt);
        
Before using this class set account name and account key in "System administration -> Setup -> Azure File Storage Accounts"

More about Azure File Storage https://docs.microsoft.com/en-us/azure/storage/storage-files-introduction

How to new create acount and mount it https://channel9.msdn.com/Blogs/MyThoughtsOnIT/How-to-create-an-SMB3-File-Share-in-Azure-Storage
