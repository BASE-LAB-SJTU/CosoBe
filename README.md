# CosoBe
A dataset is used for evaluating code search session approaches.

## Sessions
The sessions could be downloaded from [sessions.xml](https://github.com/BASE-LAB-SJTU/CosoBe/blob/master/sessions.xml)

This XML file contains 103 sessions. The session example corresponds to：
```
<session num="1" starttime="0">
    <iteration num="1" starttime="4.151">
        <query>[java]how to use stringbuffer in java</query>
        <results>	
            <result rank="1">
                <url>https://stackoverflow.com/questions/7461448/fixed-length-stringbuffer-in-java?r=SearchResults</url>
                <postid>7461448</postid>
                <title>Q: fixed-length StringBuffer in java</title>
            </result>
            ···
            <result rank="10">
                ···
            </result>
        </results>
        <clicked>
            <click num="1">
                <rank>1</rank>
                <starttime>10.7171</starttime>
                <endtime>41.6092</endtime>
            </click>
            ···
        </clicked>
    </iteration>
    ···
</session>
```

## Labels
The labels could be downloaded from [labels.csv](https://github.com/BASE-LAB-SJTU/CosoBe/blob/master/labels.csv)

This CSV file contains the relevance labels between queries and code documents in sessions. The format is :

**session_th , query_th , document_th , label**


<!-- There are three grades for relevant labels:   

| Label | Meaning | Explanation |
| --- | --- | --- | 
| 0 | irrelevant | This document does not provide useful information for the query. |
| 1 | relevant | This document provides some trivial information for the query; the relevant information must be on that page, not just promising-looking anchor text pointing to a possibly useful page. |
| 2 | highly relevant | This document provides substantial information for the query so that the developer can get a code solution. |
 -->
