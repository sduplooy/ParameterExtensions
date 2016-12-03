# ParameterExtensions
A small collection of parameter extension methods that check whether a parameter is null. In the case of strings, it will check that the parameter is not null and not empty.

# Examples
    using ParameterExtensions;
    
    public class MyClass
    {
        public void MyMethod(object obj)
        {
            obj.ThrowIfNull(nameof(obj));
            ...
        }
    
        public void MyMethod(string str)
        {
            str.ThrowIfNullOrEmpty(nameof(str));
            ...
        }
    }
    
