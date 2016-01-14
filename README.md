# flet*

expands this

```
     (flet* ((test (x) x)
             (woo (y) (test y)))
       (woo 1))
```

to this

```
     (labels ((test (x) x)
              (woo (y) (test y)))
       (woo 1))
```

Why?

All 'why' conversations around this package eventually boil down to this answer: Because.
