# CSS Transforms, Transitions, and Animations

## Transforms

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

### Transform Syntax

```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

```

### 2D Transforms

**1. 2D Rotate**

```
.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}
```

**2. 2D Scale**

```
.box-1 {
  transform: scale(.75);
}
```

**3. 2D Translate**

```
.box-1 {
  transform: translateX(-10px);
}
```

**4. 2D Skew**

```
.box-1 {
  transform: skewX(5deg);
}
```

### Combining Transforms

```
.box-1 {
  transform: rotate(25deg) scale(.75);
}
.box-2 {
  transform: skew(10deg, 20deg) translateX(20px);
}
```


## Transitions & Animations

### Transitions

The potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

There are four transition related properties in total:
`transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay`.

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
```

### Transitional Property

The `transition-property` property determines exactly what properties will be altered in conjunction with the other transitional properties.

```
.box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: 1s;
    transition-timing-function: linear;
  }
```

### Transition Duration

The duration in which a transition takes place is set using the `transition-duration` property. The value of this property can be set using general timing values, including `seconds (s)` and `milliseconds (ms)`. These timing values may also come in fractional measurements, .2s for example.

```
.box {
  background: #2db34a;
  border-radius: 6px;
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear;
}
```


## 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS

**1. Fade in**

```
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
```

**2. Change color**

**3. Grow & Shrink**

```
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
```

```
.shrink:hover
{
        -webkit-transform: scale(0.8);
        -ms-transform: scale(0.8);
        transform: scale(0.8);
}
```

**4. Rotate elements**

**5. Square to circle**

```
.circle:hover
{
        border-radius:50%;
}
```

**6. 3D shadow**

**7. Swing
**
```
@-webkit-keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
```

**8. Inset border**













