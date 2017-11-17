### Variables & Assignment

```
age = 42
first_name = 'Ahmed'
```
```
print(first_name, 'is', age, 'years old')

print(last_name)

age = age + 3
print('Age in three years:', age)
```

```
element = 'helium'
element[0]
```

```
element = 'sodium' # changing value of existing variable
element[0:3]
```

- case sensitivity
- variable naming

### Types and Type Conversion

- every value has a type
- type of variable determined/changed by its value

```
type(52)
fitness = 'average'
type(fitness)
```

```
5 - 3
'hello' + 'h'
'hello' * 4
'hello' - 'h'
```

### Built-in Functions & Help

```
'before'
print()
'after'
```

```
max(1, 2, 3)
min('a', 'A', '0')
```

```
max(1, 'a')
```

```
round(3.712) # default values
round(3.712, 1)
```

```
help(round)
```

### Libraries

### Tabular Data & DataFrames

```
import pandas

data = pandas.read_csv('data/gapminder_gdp_oceania.csv')
data
```

```
data = pandas.read_csv('data/gapminder_gdp_oceania.csv', \
index_col='country')
data
```

```
data.info()
```

```
data.columns
data.T
dir(data)
```

```
data.describe()
```

```
data = pandas.read_csv('data/gapminder_gdp_europe.csv', \
index_col='country')
data.iloc[0, 0]
data.loc["Albania", "gdpPercap_1952"]
data.loc["Albania", :]
data.loc["Albania"]
data.loc[:, "gdpPercap_1952"]
data["gdpPercap_1952"]
data.loc['Italy':'Poland', 'gdpPercap_1962':'gdpPercap_1972']
print(data.loc['Italy':'Poland', \
'gdpPercap_1962':'gdpPercap_1972'].max())
print(data.loc['Italy':'Poland', \
'gdpPercap_1962':'gdpPercap_1972'].min())

# Use a subset of data to keep output readable.
subset = data.loc['Italy':'Poland', \
'gdpPercap_1962':'gdpPercap_1972']
'Subset of data:\n', subset

# Which values were greater than 10000 ?
'\nWhere are values large?\n', subset > 10000
```

### Lists & Iteration

```
pressures = [0.273, 0.275, 0.277, 0.275, 0.276]
'pressures:', pressures
'length:', len(pressures)
```

```
# iteration
for number in [2, 3, 5]:
    number
```
