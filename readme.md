# Veebilehtede seminarid  
  
## 2. seminar  

#### Milliseid erinevaid viise leiad, et lehe sisu jagada kahte tulpa?  
  
Et jagada veebilehe sisu kahte tulpa, saab kasutada _flexbox_'i või _grid_'i.  
Eeldades, et veebilehe ülesehitus on järgnev:
```html
...
<div class='vanem-konteiner'>
    <div class='tulp-1'>...</div>
    <div class='tulp-2'>...</div>
</div>
...
```  

1. Kasutades _flexbox_'i:
```css
.vanem-konteiner {
    display: flex;
    flex-direction: row;
}
```

2. Kasutades _grid_'i:
```css
.vanem-konteiner {
    display: grid;
    grid-template-columns: 1fr 1fr
}
```

#### Miks peetakse mahukama veebilehe puhul otse HTML-elementide küljes olevat stiili (ingl inline style) halvaks tavaks?

_Inline_ stiili ei eelistata, sest see segab kaks eri keelt kokku. Samuti on raskem aru saada, mis stiil elemendile antakse, kui _css_ ja _html_ fail pole lahti samaaegselt.