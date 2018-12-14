# Annotation specification

### 1. 单行注释

```markup
# Not recommended
<div>...</div><!-- Comment Text -->	
	
<div><!-- Comment Text -->
    ...
</div>

# Recommended 
<!-- Comment Text -->
<div>...</div>
```

### 2. 模块注释

```markup
# Not recommended
<!-- S Comment Text A -->	
<div class="mod_a">
    ...
</div>
<!-- E Comment Text A -->
	
<!-- S Comment Text B -->	
<div class="mod_b">
    ...
</div>
<!-- E Comment Text B -->

# Recommended 
<!-- S Comment Text A -->
<div class="mod_a">
    ...
</div>
<!-- E Comment Text A -->
<!-- S Comment Text B -->	
<div class="mod_b">
    ...
</div>
<!-- E Comment Text B -->
```

