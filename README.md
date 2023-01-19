# CSharp

### Errors and Exceptions

```
try
{
    throw new Exception();
}
catch (Exception ex)
{
    // Get stack trace for the exception with source file information
    var st = new StackTrace(ex, true);
    // Get the top stack frame
    var frame = st.GetFrame(st.FrameCount - 1);
    // Get the line number from the stack frame
    var line = frame.GetFileLineNumber();
}
```

- [Creating and Throwing Exceptions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/exceptions/creating-and-throwing-exceptions)
