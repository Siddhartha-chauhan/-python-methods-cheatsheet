# 🐍 Python Methods Cheatsheet

A quick and easy reference for **Array**, **String**, and **Dictionary** methods in Python — with examples and outputs.  
Perfect for beginners and developers who want a clean, practical guide.

---

## 🔢 List Methods

> Lists in Python work as dynamic arrays.

| Method | Description | Example | Output |
|--------|--------------|----------|---------|
| `append(x)` | Add an element at the end | `arr = [1, 2]; arr.append(3); print(arr)` | `[1, 2, 3]` |
| `extend(iterable)` | Add multiple elements | `arr = [1]; arr.extend([2, 3]); print(arr)` | `[1, 2, 3]` |
| `insert(i, x)` | Insert at index `i` | `arr = [1, 3]; arr.insert(1, 2); print(arr)` | `[1, 2, 3]` |
| `remove(x)` | Remove first occurrence | `arr = [1, 2, 2]; arr.remove(2); print(arr)` | `[1, 2]` |
| `pop([i])` | Remove & return element | `arr = [1, 2, 3]; print(arr.pop(1))` | `2` |
| `index(x)` | Find index of `x` | `arr = [5, 7, 9]; print(arr.index(7))` | `1` |
| `count(x)` | Count occurrences | `arr = [1, 1, 2]; print(arr.count(1))` | `2` |
| `reverse()` | Reverse order | `arr = [1, 2, 3]; arr.reverse(); print(arr)` | `[3, 2, 1]` |
| `sort()` | Sort list | `arr = [3, 1, 2]; arr.sort(); print(arr)` | `[1, 2, 3]` |
| `copy()` | Return shallow copy | `arr = [1, 2]; b = arr.copy(); print(b)` | `[1, 2]` |
| `clear()` | Remove all elements | `arr = [1, 2]; arr.clear(); print(arr)` | `[]` |

---

## 🔤 String Methods

> Strings are immutable sequences of characters.

| Method | Description | Example | Output |
|--------|--------------|----------|---------|
| `upper()` | Convert to uppercase | `"hello".upper()` | `'HELLO'` |
| `lower()` | Convert to lowercase | `"HELLO".lower()` | `'hello'` |
| `capitalize()` | Capitalize first letter | `"python".capitalize()` | `'Python'` |
| `title()` | Capitalize each word | `"hello world".title()` | `'Hello World'` |
| `strip()` | Remove spaces | `"  hi  ".strip()` | `'hi'` |
| `replace(old, new)` | Replace substring | `"cat".replace("c","b")` | `'bat'` |
| `split(delimiter)` | Split into list | `"a,b,c".split(",")` | `['a', 'b', 'c']` |
| `join(iterable)` | Join iterable | `",".join(['a','b'])` | `'a,b'` |
| `find(sub)` | Find substring index | `"apple".find("p")` | `1` |
| `count(sub)` | Count occurrences | `"apple".count("p")` | `2` |
| `startswith(prefix)` | Check start | `"data".startswith("d")` | `True` |
| `endswith(suffix)` | Check end | `"data".endswith("a")` | `True` |
| `isalpha()` | Only letters | `"abc".isalpha()` | `True` |
| `isdigit()` | Only digits | `"123".isdigit()` | `True` |
| `isalnum()` | Letters + numbers | `"abc123".isalnum()` | `True` |
| `isspace()` | Only whitespace | `"   ".isspace()` | `True` |
| `swapcase()` | Swap letter cases | `"Hi".swapcase()` | `'hI'` |

### ✨ String Formatting

```python
name = "Siddhartha"
print(f"Hello, {name}!")         # f-string
print("Hello, {}!".format(name)) # format() method
```

**Output:**
```
Hello, Siddhartha!
Hello, Siddhartha!
```

---

## 🗝️ Dictionary Methods

> Dictionaries store key-value pairs — ideal for fast lookups.

| Method | Description | Example | Output |
|--------|--------------|----------|---------|
| `keys()` | Return keys | `d = {'a':1,'b':2}; print(d.keys())` | `dict_keys(['a', 'b'])` |
| `values()` | Return values | `print(d.values())` | `dict_values([1, 2])` |
| `items()` | Return key-value pairs | `print(d.items())` | `dict_items([('a', 1), ('b', 2)])` |
| `get(key, default)` | Get value safely | `print(d.get('a', 0))` | `1` |
| `update(other)` | Merge dicts | `d.update({'c':3}); print(d)` | `{'a':1, 'b':2, 'c':3}` |
| `pop(key)` | Remove key & return value | `d.pop('a')` | `1` |
| `popitem()` | Remove last pair | `d.popitem()` | `('b', 2)` |
| `clear()` | Remove all items | `d.clear(); print(d)` | `{}` |
| `copy()` | Copy dictionary | `copy_d = d.copy()` | `{'a':1, 'b':2}` |
| `setdefault(key, default)` | Add key if missing | `d.setdefault('x', 0)` | `{'a':1, 'b':2, 'x':0}` |
| `fromkeys(keys, value)` | Create new dict | `dict.fromkeys(['x','y'], 5)` | `{'x':5, 'y':5}` |

---

## ⚡ Quick Tips

- Use `dir(<object>)` to list all methods:
  ```python
  dir(list)
  dir(str)
  dir(dict)
  ```
- Lists = ordered and mutable  
- Strings = immutable text sequences  
- Dictionaries = key-value mappings  

---

## 📘 Example Summary

```python
# Array Example
arr = [1, 2, 3]
arr.append(4)
print(arr)  # [1, 2, 3, 4]

# String Example
text = "hello world"
print(text.title())  # Hello World

# Dictionary Example
person = {'name': 'Siddhartha', 'age': 22}
person.update({'city': 'Noida'})
print(person)  # {'name': 'Siddhartha', 'age': 21, 'city': 'Delhi'}
```

---


---

## 📚 References

- Content and method summaries generated with assistance from ChatGPT.  
- Additional examples and explanations adapted using Grok.  
- Tutorial: Apna College – “Python List, String & Dictionary Methods” (YouTube).  
  Available at: https://www.youtube.com/watch?v=ERCMXc8x7mc&list=PLG-efSW9nTTFzBHA81Oxq2iDM17NUkoUQ  


📚 **Author:** Siddhartha Chauhan  
📅 **Updated:** 2025  
💡 **Repo:** [`python-methods-cheatsheet`]
