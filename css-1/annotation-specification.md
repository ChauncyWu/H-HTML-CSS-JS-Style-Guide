# Annotation specification

### 1. 单行注释

```css
# Not recommended
/*Comment Text*/
.cw {
	display: block;
}
.cw {
	display: block;/*Comment Text*/
}

# Recommended 
/* Comment Text */
.cw {}

/* Comment Text */
.cw {}
```

### 2. 模块注释

```css
# Not recommended
/* Module A ---------------------------------------------------- */
.mod_a {}
/* Module B ---------------------------------------------------- */
.mod_b {}

# Recommended 
/* Module A
---------------------------------------------------------------- */
.mod_a {}


/* Module B
---------------------------------------------------------------- */
.mod_b {}
```

### 3. **文件信息注释**

```css
@charset "UTF-8";
/**
 * @desc File Info
 * @author Author Name
 * @date 2019-07-02
 */
```

