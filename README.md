<h1 align="center">
Power BI
</h1>

## Power BI Front-End vs. Back-End
![Power BI Front-End vs  Back-End](https://github.com/pratyushkiran/Power_BI/assets/124147747/27fe0db2-aa34-498a-bc47-a8b0e3f5f9e1)

## Calculated Column Best Practices
![Calculated Column Best Practices](https://github.com/pratyushkiran/Power_BI/assets/124147747/f5aa52c2-6eb6-458c-9f56-d93307aafc8b)

## Grouping & Aggregating
![grouping_aggregating](https://github.com/pratyushkiran/Power_BI/assets/124147747/fc2491b6-800c-42af-9430-061c2e49036f)

## Pivoting & Unpivoting
![pivoting_unpivoting](https://github.com/pratyushkiran/Power_BI/assets/124147747/36edf97c-120e-42f8-a8a4-6bc93f4e98fb)


## Step by Step Measure Calculation
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/9d73554d-b543-45aa-9c71-f2eabf77cbd2)


## Common DAX Function Categories  
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/76791d38-9b79-4d0f-8c26-c858de8576ac)

## Basic Math & Stats Functions
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/a660472f-d442-41b9-b8bb-869cc1e7ab8b)

## Conditional & Logical Functions
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/b39153a8-4c49-44d0-ae8f-aed1b963cc9b)

### using IF
```dax
Parent = 
IF(
    'Customer Lookup'[TotalChildren] > 0,
    "Yes", 
    "No")
```

 ## The SWITCH Function
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/0e041bba-f694-476c-a81c-a5d2bc17b0ed)

Syntax
```dax
SWITCH(Expression, Value1, Result1, ..., [Else])
```

Example to calculate Month Number
```dax
Month Number (DAX) =
    SWITCH ( // Switch statememt starts
        'Calendar Lookup'[Month Name], // from the column in which you want to apply the row context
        "January", "1", // values ...
        "Februray", "2",
        "March", "3",
        "April", "4",
        "May", "5",
        "June", "6",
        "July", "7",
        "August", "8",
        "September", "9",
        "October", "10",
        "November", "11",
        "December", "12",
        "Other" // other statement
    )
```

Example to calculate the Price Point

```dax
Price Point = 
SWITCH(
    TRUE(), 
    'Product Lookup'[ProductPrice] > 500, "High",
    'Product Lookup'[ProductPrice] > 100, "Mid-Range",
    "Low"
)
```

Examples

Objectives | Solution
:-------------------------:|:-------------------------:
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/21c898da-8816-4b5e-a1e1-138a220901d5) | ![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/e7adc63c-99e1-4740-a06a-8721ade08ad6)
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/d6043081-4ffe-42c5-91c5-912bd767c852) | ![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/7b707278-de47-49d9-bed2-6a0ed38136cb)
![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/7ea6eac7-aa23-427e-b69d-6a6208a55f0d) | ![image](https://github.com/pratyushkiran/Power_BI/assets/124147747/1ce2c36a-547c-427b-b2bf-bd1d23ee7a07)


```dax
Customer Full Name (CC) = 
'Customer Lookup'[Prefix] & " "
 & 'Customer Lookup'[FirstName] & " "
 & 'Customer Lookup'[LastName]
```


## Basic Date and Time Functions
![download](https://github.com/pratyushkiran/Power_BI/assets/124147747/f0e57567-410c-44f6-bd80-f78611985dd7)


## Filter Function
![screenshot-nimbusweb me-2023 08 18-15_16_23](https://github.com/pratyushkiran/Power_BI/assets/124147747/cb95d7d9-93a4-4622-b0cc-d6eecee67d01)

 

