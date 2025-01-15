# Countplot

# Basic Countplot
```
sns.countplot(data=data, x='Category')
plt.title('Countplot of Categories')
plt.show()
```

# Countplot with Hue
```
sns.countplot(data=data, x='Category', hue='Subcategory', palette='coolwarm')
plt.title('Countplot of Categories with Hue')
plt.show()
```

## 1. Sequential Palettes
   
Examples:
- viridis
- magma
- plasma
- cividis
- rocket
- crest
- Blues
- Greens
```
sns.countplot(data=data, x='Category', palette='magma')
```

## 2. Diverging Palettes
- Used for data with a meaningful midpoint (e.g., positive and negative values).

Examples:
- coolwarm
- Spectral
- RdBu (Red-Blue)
- PiYG (Pink-Green)
- PuOr (Purple-Orange)
```
sns.countplot(data=data, x='Category', palette='coolwarm')
```

## 3. Qualitative Palettes
- Used for categorical data with no inherent order. Good for discrete categories.

Examples:
- Set1
- Set2
- Set3
- Pastel1
- Pastel2
- Dark2
- Paired
- tab10 (Matplotlib default)
```
sns.countplot(data=data, x='Category', palette='Set2')

```
## 4. Cyclic Palettes
Used for circular or periodic data, such as angles, time of day, or days of the week.

Examples:

- twilight
- hsv
```
sns.countplot(data=data, x='Category', palette='twilight')
```

## 5. Custom Palettes
You can create custom palettes using specific colors:
```
custom_palette = ['#FF5733', '#33FF57', '#3357FF']
sns.countplot(data=data, x='Category', palette=custom_palette)
```