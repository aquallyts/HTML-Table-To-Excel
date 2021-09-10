# HTML-Table-To-Excel
Convert HTML Table to .xlsx file using EPPlus. EPPlus library only supports .xlsx(Office 2007 and above).  
The TableToExcel class uses EPPlus and Windows.Form. It can convert HTML to bytes array.  

Usage:  
```csharp
//Stream  
TableToExcel temp = new TableToExcel();  
Response.BinaryWrite(temp.process(html));  
  
//File  
TableToExcel temp = new TableToExcel();  
using (StreamWriter file = new StreamWriter("C:\\temp.xlsx"))  
{  
    file.Write(temp.process(html));  
}  
```

P.S. Solved problems of WebBrowser, changed to XmlDocument.  
