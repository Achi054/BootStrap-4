# Bootstrap-4
Web app using Bootstrap 4

Bootstrap is a front-end component library to design and develop web applications.

## Setting up Bootstrap
- Getting started through CDN
    - Goto [getbootstrap.com](https://getbootstrap.com/docs/4.3/getting-started/introduction/)
    - Copy the startup template to you code editor
- Other ways to install bootstrap are defined in [getbootstrap.com](https://getbootstrap.com/docs/4.3/getting-started/download/)

## Graphic design and responsive layout
4 principals of graphic desing<br/>
- Contrast
- Alignment 
- Repitition
- Proximity
<br/>Also know as <b>CARP</b>

## Bootstrap color names
- Primary - Blue
- Secondary - Grey
- Success - Green
- Danger - Red
- Warning - Amber
- Info - Cyan
- Dark - Black
- White - White
- Transparent - White

```
<div class="mydiv bg-primary">Hello Bootstrap</div>
    <div class="mydiv bg-secondary">Hello Bootstrap</div>
    <div class="mydiv bg-danger">Hello Bootstrap</div>
    <div class="mydiv bg-warning">Hello Bootstrap</div>
    <div class="mydiv bg-info">Hello Bootstrap</div>
```

## Bootstrap containers
Create sections with the <b>container</b> and render smooth responsiveness with <b>container-fluid</b>.

Compose table structure with <b>row</b> and <b>col</b> key words.
```
<div class="container">
        <div class="row">
            <div class="myrow col bg-primary"></div>
            <div class="myrow col bg-secondary"></div>
            <div class="myrow col bg-danger"></div>
        </div>
        <div class="row">
                <div class="myrow col bg-info"></div>
                <div class="myrow col bg-warning"></div>
        </div>
    </div>
```

## Media Break-points
- XL - 1200px
- LG - 992px
- MD - 768px
- SM - 576px
- XS - 575.98px

```
<style>
        @media(min-width: 576px){ body{ background: blue; }}
        @media(min-width: 768px){ body{ background: lightgreen; }}
        @media(min-width: 992px){ body{ background: maroon; }}
        @media(min-width: 1200px){ body{ background: cyan; }}
        @media(max-width: 575px){ body{ background: grey; }}

</style>
<body>
    <div class="text-center my-2 display-2">Bootstrap media breakpoint</div>
</body>
```

## Bootstrap grid system
The common grid layout in bootstrap is 12 column grid layout

```
<section class="container">
        <section class="row">
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
            <div class="col">Equal</div>
        </section>
    </section>
    <hr/>
    <section class="container">
        <section class="row">
            <div class="col">Auto</div>
            <div class="col-8">Auto</div>
            <div class="col-2">Auto</div>
        </section>
    </section>
    <hr/>
    <section class="container">
        <section class="row">
            <div class="col-sm order-3">First</div>
            <div class="col-sm order-1">Second</div>
            <div class="col-sm order-2">Third</div>
        </section>
    </section>
    <hr/>
    <section class="container">
        <section class="row">
            <div class="col-sm bg-warning">First</div>
            <section class="row">
                <div class="col bg-info">Second</div>
                <div class="col bg-success">Third</div>
            </section>
        </section>
    </section>
    <hr/>
    <section class="container">
        <section class="row">
            <div class="col-6 bg-success">First</div>
            <div class="col-6 bg-danger">Second</div>
        </section>
        <section class="row">
                <div class="col-4 bg-success">First</div>
                <div class="col-4 bg-danger">Second</div>
                <div class="col-4 bg-info">Third</div>
        </section>
        <section class="row">
                <div class="col-3 bg-success">First</div>
                <div class="col-3 bg-danger">Second</div>
                <div class="col-3 bg-info">Third</div>
                <div class="col-3 bg-warning">FOrth</div>
        </section>
    </section>
```

## Alignments and Offsets
Alignments set the content structure within the grid layout

```
<div class="container" style="margin-top: 20px;">
        <section class="row bg-warning align-items-end" style="height: 100px; border: 1px solid black">
            <div class="col bg-success"> Column 1</div>
            <div class="col bg-danger"> Column 2</div>
            <div class="col bg-info">Column 3</div>
        </section>
        <section class="row bg-warning align-items-center" style="height: 100px; border: 1px solid black">
            <div class="col bg-success"> Column 1</div>
            <div class="col bg-danger"> Column 2</div>
            <div class="col bg-info">Column 3</div>
        </section>
        <section class="row bg-warning align-items-start" style="height: 100px; border: 1px solid black">
            <div class="col bg-success"> Column 1</div>
            <div class="col bg-danger"> Column 2</div>
            <div class="col bg-info">Column 3</div>
        </section>
        <section class="row bg-warning" style="height: 100px; border: 1px solid black">
            <div class="col bg-success align-self-start"> Column 1</div>
            <div class="col bg-danger align-self-center"> Column 2</div>
            <div class="col bg-info align-self-end">Column 3</div>
        </section>
        <section class="row bg-warning justify-content-center" style="height: 100px; border: 1px solid black">
            <div class="col-4 bg-success"> Column 1</div>
            <div class="col-4 bg-danger"> Column 2</div>
        </section>
        <section class="row bg-warning justify-content-around" style="height: 100px; border: 1px solid black">
            <div class="col-4 bg-success"> Column 1</div>
            <div class="col-4 bg-danger"> Column 2</div>
        </section>
        <section class="row bg-warning justify-content-end" style="height: 100px; border: 1px solid black">
            <div class="col-4 bg-success"> Column 1</div>
            <div class="col-4 bg-danger"> Column 2</div>
        </section>
        <section class="row bg-warning justify-content-between" style="height: 100px; border: 1px solid black">
            <div class="col-4 bg-success"> Column 1</div>
            <div class="col-4 bg-danger"> Column 2</div>
        </section>
    </div>
```

## Padding, Display and Border
Padding and border sizes<br/>
0 - 0px<br/>
1 - 0.25px<br/>
2 - 0.5px<br/>
3 - 1px<br/>
4 - 1.5px<br/>
5 - 3px<br/>

t - margin-top or padding-top<br/>
b - margin-bottom or padding-bottom<br/>
l - margin-left or padding-left<br/>
r - margin-right or padding-right<br/>
x - left and right<br/>
y - top and bottom<br/>
blank - all way around<br/>

```
<div class="container" style="margin-top: 20px;">
    <div class="row" style="height: 100px;">
        <div class="col bg-transparent">1</div>
        <div class="col bg-secondary">2</div>
        <div class="col bg-transparent">3</div>
    </div>
    <div class="row" style="height: 100px;">
        <div class="col bg-secondary">4</div>
        <div class="col bg-transparent text-justify mt-5">
            Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries.
        </div>
        <div class="col bg-secondary">6</div>
    </div>
    <div class="row" style="height: 100px;">
        <div class="col bg-transparent">7</div>
        <div class="col bg-secondary">8</div>
        <div class="col bg-transparent">9</div>
    </div>
    <hr/>
    <span class="px-2 bg-warning d-block">Span inline element</span>
    <span class="px-2 bg-secondary">Span inline element</span>
    <hr/>
    <span class="px-2 bg-warning">Span inline element</span>
    <span class="px-2 bg-secondary">Span inline element</span>
    <div class="d-inline bg-info">Div inline element</div>
    <div class="d-inline bg-danger">Div inline element</div>
</div>
```



