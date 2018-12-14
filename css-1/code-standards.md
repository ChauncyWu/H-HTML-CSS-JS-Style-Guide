# Code Standards

### 1. 类型选择器尽量使用class，避免使用id

### 2. 省略0后没必要的单位

```css
# Recommended 
flex: 0px; /* 基于flex的组件需要一个单位 */
flex: 1 1 0px; /* 使用单位避免歧义 */
margin: 0;
padding: 0;
```

### 3. 省略没必要的0

```css
# Recommended 
font-size: .8em;
```

### 4. 使用尽可能缩写的十六进制表示法

```css
# Not recommended
color: #eebbcc;

# Recommended 
color: #ebc;
```

### 5. class名全小写，用中划线做分隔符

```css
# Not recommended
.error_status {}

# Recommended 
.ads-sample {}
```

### 7. 在选择器和开始声明块的左大括号之间使用一个空格

```css
# Not recommended
h3 {
  font-weight:bold;
}

# Recommended 
h3 {
  font-weight: bold;
}
```

### 8. 用换行分隔多个选择器

```css
# Not recommended
a:focus, a:active {
  position: relative; top: 1px;
}

# Recommended 
a:focus, 
a:active {
  position: relative; top: 1px;
}
```

### 9. 不要在url\(\)中使用引号



