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

## Flexible Box

The flex layout allows responsive elements within a container to be automatically arranged depending upon screen size.

```
<aside class="container" style="margin-top: 20px;">
    <section class="d-flex flex-row">
        <div class="p-4">One</div>
        <div class="p-4">Two</div>
        <div class="p-4">Three</div>
        <div class="p-4">Four</div>
    </section>
    <section class="d-flex flex-row-reverse">
        <div class="p-4">One</div>
        <div class="p-4">Two</div>
        <div class="p-4">Three</div>
        <div class="p-4">Four</div>
    </section>
    <section class="d-flex flex-row justify-content-center">
        <div class="p-4">One</div>
        <div class="p-4">Two</div>
        <div class="p-4">Three</div>
        <div class="p-4">Four</div>
    </section>
    <section class="d-flex flex-column">
        <div class="p-4">One</div>
        <div class="p-4">Two</div>
        <div class="p-4">Three</div>
        <div class="p-4">Four</div>
    </section>
    <section class="d-flex flex-row align-items-start">
        <div class="p-4">One</div>
        <div class="p-4">Two</div>
        <div class="p-4">Three</div>
        <div class="p-4">Four</div>
    </section>
</aside>
```

## Navigation

Navigation bar can be created by using the below code snippet

```
<div class="container">
				<nav class="navbar navbar-expand-lg navbar-light bg-transparent">
					<a class="navbar-brand" href="#">Navbar</a>
					<button
						class="navbar-toggler"
						type="button"
						data-toggle="collapse"
						data-target="#navbarNav"
						aria-controls="navbarNav"
						aria-expanded="false"
						aria-label="Toggle navigation"
					>
						<span class="navbar-toggler-icon"></span>
					</button>
					<div
						class="collapse navbar-collapse justify-content-end"
						id="navbarNav"
					>
						<ul class="navbar-nav">
							<li class="nav-item dropdown">
								<a
									class="nav-link dropdown-toggle"
									role="button"
									data-toggle="dropdown"
									href="#"
									>Dropdown</a
								>
								<div class="dropdown-menu">
									<a class="dropdown-item" href="#">Sub-link 1</a>
									<a class="dropdown-item" href="#">Sub-link 2</a>
									<a class="dropdown-item" href="#">Sub-link 3</a>
									<div class="dropdown-divider"></div>
									<a class="dropdown-item" href="#">Sub-link 4</a>
									<a class="dropdown-item" href="#">Sub-link 5</a>
									<a class="dropdown-item" href="#">Sub-link 6</a>
								</div>
							</li>
							<li class="nav-item active">
								<a class="nav-link" href="#"
									>Home <span class="sr-only">(current)</span></a
								>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#">Features</a>
							</li>
							<li class="nav-item">
								<a class="nav-link" href="#">Pricing</a>
							</li>
							<li class="nav-item">
								<a
									class="nav-link disabled"
									href="#"
									tabindex="-1"
									aria-disabled="true"
									>Disabled</a
								>
							</li>
						</ul>
					</div>
				</nav>
			</div>
```

Navigation bar is created with individual tiles using `nav-pills`. If we need to create as tabs use `nav-tabs`.

```
<div class="container m-5">
    <ul class="nav nav-tabs nav-justified">
        <li class="nav-item dropdown">
            <a
                class="nav-link dropdown-toggle"
                role="button"
                data-toggle="dropdown"
                href="#"
                >Menu Dropdown</a
            >
            <div class="dropdown-menu">
                <a class="dropdown-item" href="#">Sub-link 1</a>
                <a class="dropdown-item" href="#">Sub-link 2</a>
                <a class="dropdown-item" href="#">Sub-link 3</a>
            </div>
        </li>
        <li class="nav-item">
            <a class="nav-link active" href="#">Menu Item 1</a>
        </li>
        <li class="nav-item"><a class="nav-link" href="#">Menu Item 2</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Menu Item 3</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Menu Item 4</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Menu Item 5</a></li>
    </ul>
</div>
```

Navigation coloring is done using `navbar-<bootstrap-fillers>` and `bg-<bootstap-colors>`

```
<nav class="navbar navbar-expand-lg navbar-dark bg-info">
```

## Breadcrumb

Breadcrum composition is done using `breadcrumb` and `breadcrum-item` class

```
<div class="container m-5">
			<nav aria-label="breadcrumb">
				<ol class="breadcrumb">
					<li class="breadcrumb-item"><a href="#">Book</a></li>
					<li class="breadcrumb-item"><a href="#">GOT</a></li>
					<li class="breadcrumb-item"><a href="#">Chapter 1</a></li>
					<li class="breadcrumb-item active" aria-current="page">Page</li>
				</ol>
			</nav>
		</div>
```

## Pagination

Pagination is composed using `pagination`, `page-item` and `page-link` class

```
<div class="container m-5">
			<nav aria-label="pagination">
				<ol class="pagination">
					<li class="page-item">
						<a href="#" class="page-link"><span>&laquo</span></a>
					</li>
					<li class="page-item active"><a href="#" class="page-link">1</a></li>
					<li class="page-item"><a href="#" class="page-link">2</a></li>
					<li class="page-item"><a href="#" class="page-link">3</a></li>
					<li class="page-item">
						<a href="#" class="page-link"><span>&raquo</span></a>
					</li>
				</ol>
			</nav>
		</div>
```

## Typography

Typography can be composed through `h1 to h6, display-1 to display-4` classes

```
<div class="container m-5">
        <span class="h1 text-muted">h1 - With text muted</span><br />
        <span class="h1 text-capitalize">h1 - With text muted</span><br />
        <span class="h1 text-lowercase">h1 - With text muted</span><br />
        <span class="h1 text-uppercase">h1 - With text muted</span><br />
        <span class="display-1">display 1 - This is h1 tag</span><br />
        <span class="display-1">display 1 - This is h1 tag</span><br />
        <span class="display-1">display 1 - This is h1 tag</span><br />
        <span class="display-2">display 2 - This is h1 tag</span><br />
        <span class="display-3">display 3 - This is h1 tag</span><br />
        <span class="display-4">display 4 - This is h1 tag</span><br />
        <span class="h1">h1 - This is h1 tag</span><br />
        <span class="h2">h2 - This is h2 tag</span><br />
        <span class="h3">h3 - This is h3 tag</span><br />
        <span class="h4">h4 - This is h4 tag</span><br />
        <span class="h5">h5 - This is h5 tag</span><br />
        <span class="h6">h6 - This is h6 tag</span>
    </div>
```

Text Coloring can be composed using `text-primary, text-secondary, text-success, text-danger, text-warning, text-info, text-dark, text-body, text-black-50, text-light, text-white-50 and text-white` classes

```
<div class="container">
    <div>
        <span class="text-primary">Color primary</span><br />
        <span class="text-secondary">Color secondary</span><br />
        <span class="text-success">Color success</span><br />
        <span class="text-danger">Color danger</span><br />
        <span class="text-warning">Color warning</span><br />
        <span class="text-info">Color info</span><br />
        <span class="text-dark">Color dark</span><br />
        <span class="text-body">Color body</span><br />
        <span class="text-black-50">Color black</span><br />
    </div>
    <div class="mt-5 bg-dark w-25">
        <span class="text-light">Color light</span><br />
        <span class="text-white-50">Color white 50</span><br />
        <span class="text-white">Color white</span>
    </div>
</div>
```
