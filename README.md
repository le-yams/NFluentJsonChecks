
# NFluentJsonChecks


[NFluent](http://www.n-fluent.net/) Extensions for [JsonElement](https://learn.microsoft.com/en-us/dotnet/api/system.text.json.jsonelement).



## Check a JsonElement value

```c#
Check.That(jsonElement1).HasNullValue();
Check.That(jsonElement2).HasStringValue("foo");
Check.That(jsonElement3).HasIntValue(42);
Check.That(jsonElement4).HasBoolValue(true);
Check.That(jsonElement5).HasTrueValue();
Check.That(jsonElement6).HasFalseValue();
```


## Check the presence of a property

```c#
Check.That(jsonElement).HasProperty("foo");
```


## Check the presence and kind of a property

```c#
Check.That(jsonElement).HasProperty("foo", JsonValueKind.String);
```


## Check the presence and value of a property

```c#
Check.That(jsonElement).HasStringProperty("foo", "value");
```
