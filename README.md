# SFDataImport


<b>Data preparations mapping and pipeline design:</b>
<hr />
<code>
        ## Building ConcatId:
            1. S1 = Remove all SpecialChars* from FirstName
            2. S2 = Remove all SpecialChars* from LastName
            3. S3 = Pick first 10 Non SpecialChars* from the Address Street
            4. Build ConcatId by concatenating strings in the following order:
                        ConcatId = LOWERCASE(S1+S2+S3)
            *SpecialChars: New-line (or line break), Comma, Semicolon, Dot (or Period), Hyphen, Apostrophe, Space, Tab"
</code>

<code>
        ## Building Email+FN+LN key:
            1. S1 = Remove all SpecialChars* from FirstName
            2. S2 = Remove all SpecialChars* from LastName
            3. S3 = Email leave as is
            4. Build key by concatenating strings in the following order:
                        Email+FN+LN key = LOWERCASE(S3+S1+S2)
            *SpecialChars: New-line (or line break), Comma, Semicolon, Dot (or Period), Hyphen, Apostrophe, Space, Tab"
</code>




Reference:
Data Dictionary V2.0 : https://docs.google.com/spreadsheets/d/1FjXQeRECMETgooFskekFrrzCO1jzgogo-1M_nCODQWI/edit#gid=0

<hr />
