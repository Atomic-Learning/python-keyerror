A `KeyError`{.python} occurs when you try to access a key that doesn't exist in a dictionary or dictionary-like object. This is similar to `IndexError`{.python} with lists, but for key-based lookups instead of positional access.

# What Causes a KeyError?

KeyError is raised when you use a key that doesn't exist in a dictionary:

```py-cell
my_dict = {"name": "Alice"}
print(my_dict["age"])
```

In this example, the dictionary only has the key `"name"`{.python}, so trying to access `"age"`{.python} raises a `KeyError: 'age'`{.python}.

# String Keys are Case-Sensitive

Dictionary key lookups are also case-sensitive when a string is used as a key and must match exactly:

```py-cell
config = {"API_KEY": "secret"}

print(config["API_KEY"])
print(config["api_key"])
```
