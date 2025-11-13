# 🐍 Python Cheatsheet — Array, String & Dictionary Methods

---

## 🔢 Array Methods

> Works with `array` module or `list` (as dynamic arrays).

| Method | Description | Example |
|--------|--------------|----------|
| `append(x)` | Add an element at the end | `arr.append(10)` |
| `extend(iterable)` | Add multiple elements | `arr.extend([1, 2, 3])` |
| `insert(i, x)` | Insert element at index `i` | `arr.insert(2, 7)` |
| `remove(x)` | Remove first occurrence of `x` | `arr.remove(3)` |
| `pop([i])` | Remove and return element at index `i` | `arr.pop(0)` |
| `index(x)` | Return index of first occurrence | `arr.index(2)` |
| `count(x)` | Count occurrences of `x` | `arr.count(5)` |
| `reverse()` | Reverse the array | `arr.reverse()` |
| `sort()` | Sort the array | `arr.sort()` |
| `copy()` | Return a shallow copy | `arr.copy()` |
| `clear()` | Remove all elements | `arr.clear()` |

### 🧮 NumPy Array (Extra Useful Methods)
| Method | Description |
|--------|--------------|
| `np.sum(arr)` | Sum of all elements |
| `np.mean(arr)` | Average of elements |
| `np.max(arr)` | Maximum value |
| `np.min(arr)` | Minimum value |
| `np.sort(arr)` | Return sorted array |
| `np.unique(arr)` | Return unique elements |

---

## 🔤 String Methods

> Strings are immutable sequences of characters.

| Method | Description | Example |
|--------|--------------|----------|
| `upper()` | Convert to uppercase | `"hello".upper()` → `"HELLO"` |
| `lower()` | Convert to lowercase | `"HELLO".lower()` → `"hello"` |
| `capitalize()` | Capitalize first letter | `"python".capitalize()` |
| `title()` | Capitalize each word | `"hello world".title()` |
| `strip()` | Remove spaces (start/end) | `"  hi  ".strip()` |
| `lstrip()` | Remove left spaces | `"  hi".lstrip()` |
| `rstrip()` | Remove right spaces | `"hi  ".rstrip()` |
| `replace(old, new)` | Replace substring | `"cat".replace("c","b")` → `"bat"` |
| `split(delimiter)` | Split into list | `"a,b,c".split(",")` → `['a','b','c']` |
| `join(iterable)` | Join iterable into string | `",".join(['a','b'])` → `"a,b"` |
| `find(sub)` | Find first index of substring | `"apple".find("p")` → `1` |
| `count(sub)` | Count substring occurrences | `"apple".count("p")` → `2` |
| `startswith(prefix)` | Check start | `"data".startswith("d")` → `True` |
| `endswith(suffix)` | Check end | `"data".endswith("a")` → `True` |
| `isalpha()` | True if only alphabets | `"abc".isalpha()` |
| `isdigit()` | True if only digits | `"123".isdigit()` |
| `isalnum()` | True if letters & numbers | `"abc123".isalnum()` |
| `isspace()` | True if only whitespace | `"   ".isspace()` |
| `swapcase()` | Swap letter cases | `"Hi".swapcase()` → `"hI"` |

---

## 🗝️ Dictionary Methods

> Dictionaries store data as **key-value pairs**.

| Method | Description | Example |
|--------|--------------|----------|
| `keys()` | Return all keys | `my_dict.keys()` |
| `values()` | Return all values | `my_dict.values()` |
| `items()` | Return key-value pairs | `my_dict.items()` |
| `get(key, default)` | Get value by key | `my_dict.get('age', 0)` |
| `update(other_dict)` | Add/merge another dict | `my_dict.update({'city':'Delhi'})` |
| `pop(key)` | Remove key and return value | `my_dict.pop('age')` |
| `popitem()` | Remove and return last pair | `my_dict.popitem()` |
| `clear()` | Remove all items | `my_dict.clear()` |
| `copy()` | Return shallow copy | `copy_dict = my_dict.copy()` |
| `setdefault(key, default)` | Insert key if not present | `my_dict.setdefault('status','active')` |
| `fromkeys(keys, value)` | Create new dict from keys | `dict.fromkeys(['a','b'], 0)` → `{'a':0,'b':0}` |

---

## 🧠 Quick Notes

- **Arrays** → Use when dealing with numerical data or lists of same type.  
- **Strings** → Use string methods for clean text processing.  
- **Dictionaries** → Fast lookup tables; ideal for mapping relationships.  

---

✅ **Pro Tip:**  
Use `dir(object)` to list all available methods for any data type.  
Example:  
```python
dir(str)      # Lists all string methods
dir(list)     # Lists all list/array methods
dir(dict)     # Lists all dictionary methods
