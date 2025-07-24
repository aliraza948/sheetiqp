# SheetIQ

> Python SDK for reading and writing to Google Sheets using [docapi.datafetchpro.com](https://docapi.datafetchpro.com)

## 🚀 Installation

```bash
pip install sheetiq
```

##  Initlization

```py
from sheetiq.sheetiq import SheetIQ
sheet=SheetIQ({"token":"YOUR_BEARER_TOKEN"})
```

## Get Sheet Data

```py
sheet.get_sheet({"id":"1jNPCbbYGT49dlXCeWkAoutazh3Cp2awsJyXnWyAKZ8E","range":"Sheet1"})
```

## Append Data on Sheet

```py
res = sheet.update_sheet({
    "id": "1jNPCbbYGT49dlXCeWkAoutazh3Cp2awsJyXnWyAKZ8E",
    "range": "Sheet1",
    "type": "append",
    "data": [["example@gmail.com"]]
})
```

## Update Data on Sheet

```py
res = sheet.update_sheet({
    "id": "1jNPCbbYGT49dlXCeWkAoutazh3Cp2awsJyXnWyAKZ8E",
    "range": "Sheet1",
    "type": "update",
    "data": [["example@gmail.com"]]
})
```

