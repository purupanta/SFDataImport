# SFDataImport (Underdevelopment... please check back)


<b>Data preparations mapping and pipeline design:</b>
<hr />

#### Major Operatiions <sup>2</sup> :
        a. Contact: Lookup contact based on criteria (Ref.2). Create contact if not found
        b. RFIForm: No lookup on RFIForm. Always Create RFI For every prospect
        c. Recruitment: Lookup Recruitment based on criteria(Ref.2). Create if not found. Update the following fieds if Recruitment is found:
                Id (The existing Recruitment's Id)
                Student_Type__c,
                HS_GPA__C,
                Source__c,
                Term__c,
                External_System__c,
                Contact__c,
                Secondary_Program_or_Major_of_Intrest__c,
                Program_Major_of_Interest__c,
                RecordTypeId,
                HS_Name__C,
                HS_CEEB_Code__c,
                Inquiry_Date__c

#### Data Mapping and Business Logic
        Ref. 1

#### Building ConcatId:
        1. S1 = Remove all SpecialChars* from FirstName
        2. S2 = Remove all SpecialChars* from LastName
        3. S3 = Pick first 10 Non SpecialChars* from the Address Street
        4. Build ConcatId by concatenating strings in the following order:
        ConcatId = LOWERCASE(S1+S2+S3)
        *SpecialChars: New-line (or line break), Comma, Semicolon, Dot (or Period), Hyphen, Apostrophe, Space, Tab
        
#### Building Email+FN+LN key:
        1. S1 = Remove all SpecialChars* from FirstName
        2. S2 = Remove all SpecialChars* from LastName
        3. S3 = Email leave as is
        4. Build key by concatenating strings in the following order:
        Email+FN+LN key = LOWERCASE(S3+S1+S2)
        *SpecialChars: New-line (or line break), Comma, Semicolon, Dot (or Period), Hyphen, Apostrophe, Space, Tab
<hr /><br />

#### References:
1. "Data Dictionary V2.0", URL: https://docs.google.com/spreadsheets/d/1FjXQeRECMETgooFskekFrrzCO1jzgogo-1M_nCODQWI/edit#gid=0
2. Contacts, RFIForms, Recruitments operations in flow, URL: https://lucid.app/lucidchart/45222f8d-8a4a-4224-950e-4c3b47487be8/edit?page=0_0&invitationId=inv_ff90952b-77ae-4e88-bce0-9449845de378#
3. DataLoad Log, URL: https://uky.lightning.force.com/lightning/o/DataLoadLog__c/list

<hr />
