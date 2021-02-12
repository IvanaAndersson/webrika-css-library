# CSS writing style guide
The team style guide should always win over your own personal preferences. Consistency is important.

## Selector specificity

### 1. Avoid overly-specific selectors

avoid selectors such as:
```
.header.flex.mt-10 {}

.header p a span {}
```
instead write a class for the nested element you want to taget.

### 2. Don't use ID selectors
Except when you need to override an id selector from a Shopify theme


### 3. Put multiple selectors on separate lines

```
h1,
h2,
h3 {
  font-family: sans-serif;
  text-align: center;
}
```


## Class naming convention guidelines

### Dash instead of underscore
```
.class-name  

instead of 

.class_name
```

### 