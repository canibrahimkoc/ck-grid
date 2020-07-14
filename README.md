# ck-grid

###Demo link : <https://codepen.io/canibrahimkoc/pen/abdaZbz>

####Html code

```html
    <div class="page-container">
        <div class="row">
            <div class="col">test</div>
            <div class="col">test</div>
            <div class="col">test</div>
            <div class="col">test</div>
            <div class="col">test</div>
            <div class="col">test</div>
        </div>
        <div class="row">
            <div class="col">test</div>
            <div class="col">test</div>
            <div class="col">test</div>
        </div>
        <div class="row">
            <div class="col">test</div>
            <div class="col">test</div>
        </div>
    </div>
```

####Sass code

```sh
    @include container;
    
    .row {
        @include row;

        &:nth-child(1) {
            .col {
                @include grid(6,1);
            }
        }

        &:nth-child(2) {
            .col {
                @include grid(3,1);
            }
        }

        &:nth-child(3) {
            .col {
                @include grid(2,1);
            }
        }
    }
```
