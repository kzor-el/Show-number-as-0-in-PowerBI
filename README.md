# Show-number-as-zero-in-PowerBI
How to show a null number as zero in PowerBI

When a calucation equals zero on PowerBIit will display with the word BLANK.

To enable the figure to show as a numeric zero (0) a the following variable return fucntion to the calculation.

i.e. 

Measure = Var a = "SharePoint List Name'[Column Name] / "SharePoint List Name'[Column Name] 
          Return (if(ISBLANK(a) || ISERROR(a),0,a))
