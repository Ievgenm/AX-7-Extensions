URLUtility class extension to create "deep" links. Deep links allow to open a form with specific record.

Usage example:

    public static void main(Args _args)
    {
        Map indexFieldValuesMap = new Map(Types::String, Types::String);
        indexFieldValuesMap.insert(fieldStr(VendTable, AccountNum), '1002');
 
        Box::info(URLUtility::generateRecordUrl(menuItemDisplayStr(VendTable), MenuItemType::Display, identifierStr(VendTable), indexFieldValuesMap, 'usmf'));
    }
