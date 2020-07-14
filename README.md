# ck-grid

Demo: <https://codepen.io/canibrahimkoc/full/abdaZbz>

ck-grid.scss lets you style embedded grid using SCSS. It's as simple as declaring all the required variables and importing the `ck-grid.scss` file into your Sass project.

## Options

```scss

$wrapper-breakpoints: (xs:576px, sm:576px, md:768px, lg:992px, xl:1200px) !default;
$wrapper-width: (xs:100%, sm:100%, md:100%, lg:960px, xl:1140px) !default;
$wrapper-gutter: (xs:10px, sm:10px, md:10px, lg:15px, xl:15px) !default;

```

## Html Example

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

## Sass Example

```S
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



## Responsive Example

```S
    @include mq(xl,max) {
        //
    }
    @include mq(xl,min) {
        //
    }
    @include mq(lg,max) {
        //
    }
    @include mq(lg,min) {
        //
    }
    @include mq(md,max) {
        //
    }
    @include mq(md,min) {
        //
    }
    @include mq(sm,max) {
        //
    }
    @include mq(sm,min) {
        //
    }
    @include mq(xs,max) {
        //
    }
    @include mq(xs,min) {
        //
    }
```
