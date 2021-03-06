---
-api-id: T:Windows.Foundation.IReference`1
-api-type: winrt interface
---

<!-- Interface syntax.
public interface IReference<T> : Windows.Foundation.IPropertyValue
-->

# Windows.Foundation.IReference<T>

## -description
Enables arbitrary enumerations, structures, and delegate types to be used as property values.



> **.NET**
> This interface appears as [Nullable&lt;T&gt;](XREF:TODO:T:System.Nullable`1).



> **C++/CX**
> This interface appears as [Platform::IBox&lt;T&gt;](XREF:TODO:774df45d-f8a7-45a3-ae24-eecc3c681040)

## -remarks
When programming with .NET, this interface is hidden and developers should use the [Nullable&lt;T&gt;](XREF:TODO:T:System.Nullable`1) class. All Windows Runtime members where the basic IDL signature shows [IReference](ireference_1.md) (with a constraint) are instead exposed using the nullable syntax of the nullable value type (for example, **?bool**).

When programming with C++/CX, this interface is hidden and developers should use the [Platform::IBox&lt;T&gt;](XREF:TODO:774df45d-f8a7-45a3-ae24-eecc3c681040) interface. All Windows Runtime members where the basic IDL signature shows [IReference](ireference_1.md) (with a constraint) are instead exposed using [Platform::IBox&lt;T&gt;](XREF:TODO:774df45d-f8a7-45a3-ae24-eecc3c681040) with the template as a particular value type. This is how C++/CX implements nullable value types. For more info, see [Value classes and structs (C++/CX)](XREF:TODO:262a0992-9721-4c02-8297-efc07d90e5a4).

Because both .NET and C++/CX have projection equivalents, don't implement this interface unless you are using WRL and/or writing code for a Windows Runtime component and need a nullable value type.

### Interface inheritance

[IReference&lt;T&gt;](ireference_1.md) inherits [IPropertyValue](ipropertyvalue.md). Types that implement [IReference&lt;T&gt;](ireference_1.md) also implement the interface members of [IPropertyValue](ipropertyvalue.md).

## -examples

## -see-also
[IPropertyValue](ipropertyvalue.md), [Nullable&lt;T&gt;](XREF:TODO:T:System.Nullable`1), [Platform::IBox&lt;T&gt;](XREF:TODO:774df45d-f8a7-45a3-ae24-eecc3c681040), [Value classes and structs (C++/CX)](XREF:TODO:262a0992-9721-4c02-8297-efc07d90e5a4)